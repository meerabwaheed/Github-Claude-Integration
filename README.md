# Github-Claude-Integration

{
  "name"       : "Meerab Waheed",
  "role"       : "Full Stack Developer",
  "location"   : "Pakistan",
  "email"      : "meerabdev@gmail.com",
  "github"     : "github.com/meerabwaheed",
  "experience" : "Aspiring Software Engineer",
  "openToWork" : true
}
What Is This Guide About?
Claude Code is a powerful AI coding assistant that normally costs money because it uses Anthropic's cloud API. But with a tool called Ollama, you can run it completely free on your own computer — no internet needed, no rate limits, and your code never leaves your machine.
This guide walks you through the full setup from scratch, step by step.


What You Need Before Starting
Check the following before you begin:
A PC running Windows (with Git for Windows or WSL), macOS, or Linux
At least 8 GB of RAM (16 GB or more recommended)
10–35 GB of free storage space (for the AI model)
A working internet connection just for the initial downloads

Good news: You do NOT need an Anthropic account, API key, or credit card for this setup.



Step 1 — Install Ollama
Ollama is the software that runs AI models locally on your computer. Think of it as the engine that powers everything.
On Mac or Linux
Open your Terminal and run this command:
curl -fsSL https://ollama.com/install.sh | sh
On Windows
Go to https://ollama.com and download the Windows installer (.exe file). Run it just like any normal Windows app installation.
Verify the installation
After installing, run this in your terminal to confirm it worked:
ollama --version
You should see a version number like ollama version 0.14.0 or higher.
Note: Ollama v0.14.0 or newer is required for Claude Code compatibility.

Step 2 — Download an AI Model
Now you need to download an AI model that will do the actual coding work. Pick one based on how powerful your computer is:

Your PC
Recommended Model
Command to Run
Size
Low-end (8 GB RAM)
Llama 3.2 3B
ollama pull llama3.2:3b
~2 GB
Mid-range (16 GB RAM)
Qwen2.5-Coder 7B
ollama pull qwen2.5-coder:7b
~5 GB
Powerful (32 GB+ RAM)
Qwen2.5-Coder 32B
ollama pull qwen2.5-coder:32b
~20 GB
Any PC (free cloud)
Qwen3-Coder
ollama pull qwen3-coder
cloud


Example — if you have a powerful PC, run:
ollama pull qwen2.5-coder:32b
The download will take a few minutes depending on your internet speed. You will see a progress bar.
Tip: For best results with Claude Code, your model should support at least 32,000–64,000 tokens of context. Qwen2.5-Coder and Qwen3-Coder both support this well.


