🧠 Local LLM Chat Demo (using Transformers.js)
A lightweight local web app that lets you ask questions or generate text using a Transformers.js model (GPT‑2 by default) entirely in your browser.

📁 Project Description
This project sets up a minimal frontend-only chatbot using the @xenova/transformers JavaScript library. It runs fully client-side (in your browser) and uses GPT-2 or another Hugging Face model to generate responses. No backend is required — just a static file server.

🛠️ Step 1: Project Setup (Installation)
Open your terminal or PowerShell and navigate to your working folder:

cd C:\Projects\ai-projects\llm_local3

Initialize a Node.js project:

npm init -y

Install the Transformers.js library:

npm install @xenova/transformers

This only installs the JavaScript dependencies. The actual model (e.g., GPT-2) is downloaded by the browser the first time the app is used. That download is around 500 MB.

🚀 Step 2: Run the Project
Still in the same folder (C:\Projects\others_projects\llm_local3), start a local web server:

npx serve .

You should see something like:

Serving!
Local: http://localhost:3000

Open that address (http://localhost:3000) in your browser.

💬 How It Works
When you open the HTML file in the browser, the GPT-2 model is downloaded and cached locally.

You type a question like:
"Who discovered America?" or "2 + 3 ="

The model will generate text based on your prompt, right in the browser.

There’s no connection to external APIs — everything happens locally.

✅ Summary
Install:

npm init -y

npm install @xenova/transformers

Run:

npx serve .

Visit http://localhost:3000 in your browser

The app loads a GPT-2 model and allows you to chat with it directly in the browser. You can change the model in your HTML by editing the line with pipeline('text-generation', 'Xenova/gpt2').

