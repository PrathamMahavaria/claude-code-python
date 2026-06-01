# Claude Code Python

A mini AI coding agent built in Python using OpenRouter and Claude.

This project implements:

* iterative agent loops
* OpenAI-compatible tool calling
* filesystem interaction
* bash command execution

Built as part of the Codecrafters "Build Your Own Claude Code" challenge.

---

## Features

* Read files using the `Read` tool
* Create and modify files using the `Write` tool
* Execute terminal commands using the `Bash` tool
* Multi-step reasoning using an agent loop
* Tool execution feedback system
* JSON-based tool schemas

---

## Tools Supported

### Read Tool

Reads file contents and sends them back to the LLM.

### Write Tool

Creates or updates files based on LLM instructions.

### Bash Tool

Executes terminal commands using Python's `subprocess` module.

---

## Tech Stack

* Python
* OpenRouter API
* Claude Haiku
* JSON tool schemas
* subprocess module

---

## Project Structure

```text
claude-code-python/
│
├── app/
│   └── main.py
├── README.md
├── your_program.sh
├── pyproject.toml
└── .gitignore
```

---

## Example Usage

Run the agent:

```bash
./your_program.sh -p "Create a hello.py file and run it"
```

Example prompts:

```bash
./your_program.sh -p "Read README.md"
```

```bash
./your_program.sh -p "Create a python file that prints hello world"
```

```bash
./your_program.sh -p "List all files in the current directory"
```

---

## Concepts Learned

This project helped me learn:

* AI agent loops
* OpenAI-compatible tool calling
* subprocess execution
* filesystem manipulation
* structured JSON messaging
* LLM orchestration
* iterative reasoning systems

---

## Codecrafters Challenge

[![progress-banner](https://backend.codecrafters.io/progress/claude-code/9f0d3951-fae3-4f4a-b818-089bcbc4ca87)](https://app.codecrafters.io/users/codecrafters-bot?r=2qF)

This repository is based on the Codecrafters
["Build Your Own Claude Code"](https://codecrafters.io/challenges/claude-code)
challenge.

Claude Code is an AI coding assistant that uses Large Language Models (LLMs)
to understand code and perform actions through tool calls.

The challenge walks through:

* HTTP APIs
* OpenAI-compatible tool calling
* agent loops
* multi-tool orchestration
* AI coding assistants

---

## Running Locally

Install dependencies:

```bash
pip install -r requirements.txt
```

Set environment variables:

```bash
export OPENROUTER_API_KEY=your_api_key
export OPENROUTER_BASE_URL=https://openrouter.ai/api/v1
```

Run the project:

```bash
./your_program.sh -p "Your prompt here"
```
