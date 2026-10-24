# Workflow Files

This directory contains the n8n workflow for the Local AI Research Assistant.

# Workflow Overview

The workflow connects:

- **Chat Trigger:** Receives user messages.
- **AI Agent:** Coordinates the response and decides when to use tools.
- **Ollama + Qwen3 4B:** Runs the language model locally.
- **Calculator:** Performs calculations.
- **Wikipedia:** Retrieves general reference information.

## Requirements

- n8n
- Ollama
- The `qwen3:4b` model
- The relevant n8n LangChain nodes

## Security

Workflow exports should be reviewed and sanitized before sharing. Do not publish credentials, API keys, private endpoints, or execution data.

This project is a learning project; tool outputs should be verified for accuracy.
