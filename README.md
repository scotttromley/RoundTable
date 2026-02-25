# RoundTable

> A single-file, zero-build web application for orchestrating complex, multi-persona LLM prompts and managing iterative synthesis rounds.

**RoundTable** is a lightweight, client-side tool designed to help prompt engineers and developers manually orchestrate "Mixture of Experts" (MoE) style workflows. It allows you to gather responses from multiple AI personas (or "friends"), synthesize them, and iteratively build complex prompts without needing a backend.

## ✨ Key Features

* **Zero-Dependency Setup:** Runs entirely in the browser. Just open the `index.html` file. 
* **Multi-Persona Management:** Easily add, name, and remove multiple "friends" (personas) to paste their individual LLM outputs.
* **Iterative Round Tracking:** Keeps track of your prompting rounds with default, built-in instructions for sequential evaluation (e.g., Round 1: Synthesize solutions; Round 2: Rank, fix, and evaluate).
* **One-Click Prompt Compilation:** Automatically concatenates your main instructions with the formatted outputs of all your "friends" into a clean Markdown structure. 
* **Keyboard Shortcuts:** Press `Cmd + Enter` (or `Ctrl + Enter`) to quickly build your prompt without moving your mouse.
* **Live Preview & Copy:** Toggle between the raw text prompt and a rendered HTML preview. Copy the final prompt to your clipboard with a single click.
* **Local Persistence:** Automatically saves your state, session names, and prompt history to your browser's `localStorage` so you never lose your work on accidental refresh.
* **Session & History Management:** Save different workspaces as named sessions, load previous sessions, and browse an expandable, timestamped history of every prompt you've built.

## 🚀 How to Use

1. Clone this repository or download the `index.html` file directly.
2. Double-click the file to open it in any modern web browser.
3. Enter an **Instruction for this round** (or leave the pre-populated default).
4. Click **+ Friend** to add personas, give them aliases (e.g., "GPT-4", "Claude", "Expert A"), and paste their respective responses into the text areas.
5. Click **Build prompt ⌘↵** to compile the data into a single, cohesive prompt ready to be fed back into your LLM of choice.

## 🛠️ Built With

* **HTML/JavaScript** - Core logic and structure.
* **[Tailwind CSS](https://tailwindcss.com/)** (via CDN) - For rapid, utility-first styling.
* **[Marked.js](https://marked.js.org/)** (via CDN) - For rendering the compiled Markdown prompt into an HTML preview.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
