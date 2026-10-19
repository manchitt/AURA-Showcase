# AURA

### A personal, local AI coding assistant for macOS

AURA is a native macOS application I built to explore how a local language model can support both everyday conversation and hands-on coding. It combines a SwiftUI interface with Ollama and uses a single model, **Qwen 3.5 9B**, for chat and project tasks.

## What it does

- **Local AI chat:** Ask questions, discuss code, and continue conversations using a model served by Ollama on the Mac.
- **Coding agent:** Open a project and ask AURA to inspect files, create or update code, and help build basic projects through a step-by-step workflow.
- **File and command actions:** The agent can list, read, and write project files and propose shell commands. Existing-file overwrites and commands require approval in the current implementation.
- **Native workspace:** A SwiftUI interface brings together chat, a project file browser, an editor, and activity updates.
- **Attachments and saved chats:** The app supports file and image attachments, PDF text extraction, session file memory, and locally saved conversations.
- **Fast and Deep Think modes:** Chat can use a concise response mode or enable model thinking for more involved questions.

## How it works

AURA sends requests to Ollama's local chat API. A simple keyword-based router chooses between a conversational flow and an agent flow when a project folder is open. The agent asks the model for structured actions, executes supported actions, and feeds the results back to the model for the next step. Both flows use the same model.

## Technology

**Swift · SwiftUI · macOS · Ollama · Qwen 3.5 9B · Local inference**

## Project status

AURA is a personal, evolving project. Basic chat and project-building workflows have been used successfully; more complex tasks and edge cases are still being tested. Model responses and generated code should be reviewed.

## Source availability

This repository is a **project showcase only**. AURA's source code and application are private and are not distributed here.
