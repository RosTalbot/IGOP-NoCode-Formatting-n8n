# 🥞 IGOP – International GPT of Pancakes

A no-code AI agent built during the Lonely Octopus AI Agent Bootcamp (Week 1) that lets users request regional pancake recipes from around the world. The agent responds with formatted, culturally-relevant HTML recipes powered by GPT-4.


## 🌍 Project Goal

Build a no-code workflow in [n8n](https://n8n.io) that:

1. Collects user input for a country or culture (e.g., Morocco, Thailand, France)
2. Passes it to GPT-4 with a detailed HTML prompt
3. Returns a real pancake recipe using clean, moderately styled formatting
4. Displays the result inside a web form view


## 🧠 Why This Matters

Many LLM outputs are plain-text walls or markdown blobs. This project proves that:
- **HTML output can be structured + stylish**, even from a no-code AI agent
- GPT can follow very specific formatting instructions when prompted well
- Even beginner-friendly tools like n8n can deliver *delightful* user experiences


## 🛠️ Tools Used

- **n8n**: Workflow builder and form interface
- - **n8n Form Trigger**: Captures the country/culture input from users
- - **n8n Form Node**: Displays the styled recipe result in-browser
- **OpenAI (GPT-4o)**: Language model generating the recipe


## 💡 Prompt Design Highlights

The prompt instructed GPT to return:
- The dish name and country
- Ingredient list (`<ul>`)
- Step-by-step prep (`<ol>`)
- Optional cultural fun fact (`<p>`)
- Cheeky tone and warm sign-off  
- **Clean HTML only** – no markdown, no triple-backticks

It also included constraints like:
- No AI disclaimers
- No invented mashups
- Real, traditional pancake recipes only
- No follow-up questions

## 📁 Files Included

- [`igop_nocode_pancake_agent_n8n_workflow.json`](./igop_nocode_pancake_agent_n8n_workflow.json) – Full n8n export of the working agent  
- [`igop_gpt_prompt_sassy_pancake_agent.md`](./igop_gpt_prompt_sassy_pancake_agent.md) – The full prompt used to generate culturally accurate, sassy recipes  
- [`example-output_brazilian-pancake.html`](./example-output_brazilian-pancake.html) – Sample output in clean HTML format  
- [`screenshots/`](./screenshots/) – Inbox and formatting previews  
- [`README.md`](./README.md) – You’re reading it!


## 🎉 Sample Output

> “Today, we’re flipping our way into Morocco! These **Baghrir**, or ‘thousand-hole pancakes’, are light, spongy, and perfect for soaking up honey butter...”

*Output includes full ingredients + prep method, fun fact, and a fabulous sign-off.*


## 🚀 Want to Try It?

Fork the repo or import the `.json` file into your own n8n instance to play with the agent. No coding required — just a working OpenAI key and a few minutes to customize.


## 🙏 Credits

This project was created by Ros Talbot, with creative prompt design, HTML formatting tricks, and wild brunch energy. 🧇✨
