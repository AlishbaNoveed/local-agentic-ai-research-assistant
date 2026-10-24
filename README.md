# Local Agentic AI Research Assistant

A beginner-friendly, locally running AI agent built with **n8n, Ollama, and Qwen3 4B**. This project explores how an AI agent can respond to user questions and use external tools to support its answers.

## Project Overview

Unlike a basic chatbot that only generates text, this project uses an AI Agent node connected to tools that it can call when appropriate.

### Architecture

- **n8n:** Workflow orchestration and chat interface
- **Ollama:** Runs the language model locally
- **Qwen3 4B:** Language model used by the agent
- **Calculator:** Handles mathematical calculations
- **Wikipedia:** Provides access to general reference information

## Workflow

![Local AI Research Assistant workflow](<screenshots/Agent Image 1.jpeg>)

The chat trigger receives a message and passes it to the AI Agent. The agent uses the local language model and can call the Calculator or Wikipedia tool when needed.

## Example Capabilities

- Answer general questions
- Perform calculations using the Calculator tool
- Retrieve general reference information using Wikipedia
- Combine a language model with tools in a visual workflow

## Technology Stack

`n8n` · `Ollama` · `Qwen3 4B` · `AI Agents` · `Tool Calling`

## Project Structure

```text
local-agentic-ai-research-assistant/
├── README.md
├── screenshots/
│   ├── README.md
│   └── workflow-overview.png
└── workflows/
    ├── README.md
    └── research-agent.json
```

## Run Locally

1. Install [n8n](https://n8n.io/) and [Ollama](https://ollama.com/).
2. Download the `qwen3:4b` model using Ollama.
3. Import `workflows/research-agent.json` into n8n.
4. Configure the Ollama credential and connection for your environment.
5. Open the workflow chat and test the agent.

Exact setup may vary by operating system and n8n deployment method.

## Current Limitations

- Responses depend on the local model's capabilities.
- Wikipedia results should be verified when accuracy matters.
- The agent does not guarantee comprehensive research or fully sourced answers.
- This is a learning project, not a production-ready research system.

## Learning Goals

This project is part of my journey into agentic AI, tool calling, local language models, and workflow automation.

## Security

No credentials, API keys, or passwords should be committed to this repository. Review workflow exports and screenshots before sharing updates.

## License

This project is shared for learning and educational purposes. A formal license can be added if reuse permissions need to be defined.
