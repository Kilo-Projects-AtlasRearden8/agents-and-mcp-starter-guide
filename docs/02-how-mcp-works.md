# How MCP Servers Connect Local Files and Tools

MCP stands for the **Model Context Protocol**. That is a formal name for a simple idea: a standard way for AI tools to connect to the files and programs already on your computer.

## The problem MCP solves

Before MCP, every AI tool that wanted to read your files needed its own custom connection. One tool for your notes, another for your calendar, another for your code. Each connection was built differently, so they did not work together, and each one had to be built from scratch.

MCP is like a universal plug. Instead of every AI tool inventing its own way to reach your files, every tool speaks the same language: MCP.

## The three parts of an MCP setup

An MCP connection has three pieces:

| Part | What it is | Analogy |
|------|-----------|---------|
| **AI client** | The AI tool you use (a chat app, a coding assistant, an agent) | You |
| **MCP server** | A small program that connects the AI to a specific set of files or tools | A helper with keys to one room |
| **Local resource** | The files or tools on your computer (your documents folder, a calendar app, a local database) | The room |

The AI client asks the MCP server for something ("read this file," "list my documents"), and the MCP server does it on the AI's behalf. The AI never touches your files directly — the server is in between.

## stdio: the simplest connection

MCP servers can connect in different ways. The simplest one is called **stdio** (standard input/output). The MCP server runs right on your computer, and the AI client talks to it through the same channel programs use to print text and read input.

Why stdio first?

- It runs entirely on your computer. Nothing leaves your machine unless you want it to.
- It is easy to set up. No websites, no accounts, no API keys.
- It is a great way to learn how MCP works before trying anything more advanced.

## What an MCP server can connect to

An MCP server is just a small program, so it can connect to almost anything. Common examples for beginners:

- **Local files** — read files in a folder you choose
- **Local notes** — read your markdown or text files
- **A calendar** — list upcoming appointments
- **A task list** — read and check off to-dos

Each MCP server usually does one thing well. You pick the servers you need.

## Quick checklist: understanding an MCP server before you run it

- [ ] What files or tools will this server reach?
- [ ] Does it run on my computer, or does it send data somewhere else?
- [ ] Who made the server, and do I trust them?
- [ ] Can I limit it to one folder instead of my whole computer?

## Glossary

- **MCP (Model Context Protocol)**: A standard way for AI to connect to files and tools.
- **MCP server**: A small program that connects an AI client to a local resource.
- **AI client**: The AI tool you use that speaks MCP.
- **stdio**: A simple way for programs to exchange text, running on your own computer.

---

*Next: [Running your first stdio server](03-running-your-first-stdio-server.md)*

*Published by Asdale Dynamics, LLC — beginner-friendly AI education, books, and tools.*
