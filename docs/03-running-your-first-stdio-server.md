# Running Your First stdio Server

This chapter walks you through running your first MCP server over stdio. No programming is required. Every command below is something you copy and paste into your terminal.

A **stdio server** runs entirely on your own computer. The AI client talks to it through text, and your files never have to leave your machine.

## Before you start: a safety-first folder

Because this is your first time, we will give the server access to exactly one folder — nothing else. Create a practice folder somewhere easy to find, like your Documents folder, and put a few harmless files in it (notes you do not mind sharing, a grocery list, a practice document).

**Do not** point your first server at your whole computer, your tax folder, or anything with passwords in it.

## What you need

- A computer with a terminal (Command Prompt or PowerShell on Windows, Terminal on Mac, Terminal on Linux)
- An AI client that supports MCP stdio servers (for example, Claude Desktop, Cursor, or any MCP-compatible chat app)
- About 15 minutes

## Step-by-step checklist

### Step 1: Create your practice folder

- [ ] Open your file explorer
- [ ] Create a new folder named `mcp-practice` inside your Documents folder
- [ ] Inside it, create two text files: `grocery-list.txt` and `notes.txt`
- [ ] Type something simple in each file so you will recognize it later

### Step 2: Install an MCP stdio server

There are many MCP servers available. For your first one, pick a simple "local files" server. A common choice is the official filesystem server (it reads files in folders you allow). You install it with one command, depending on what your computer uses:

- **If your computer uses Node.js** (most common): copy and paste this into your terminal:

```
npx -y @modelcontextprotocol/server-filesystem /Users/you/Documents/mcp-practice
```

On Windows, replace the path with something like:

```
npx -y @modelcontextprotocol/server-filesystem C:\Users\you\Documents\mcp-practice
```

- **If you do not have Node.js**: install it first from nodejs.org, then run the command above.

> The `npx` command downloads the server and runs it. It does not change your system permanently.

### Step 3: Connect your AI client to the server

Open your AI client's settings and look for "MCP," "Model Context Protocol," or "Servers." Add a new stdio server with these details:

- **Name:** My First MCP Server
- **Command:** `npx`
- **Arguments:** `-y`, `@modelcontextprotocol/server-filesystem`, and the full path to your `mcp-practice` folder

Save the setting. Your AI client will start the server and talk to it through stdio.

### Step 4: Test it

Ask your AI client something like:

> "List the files in my mcp-practice folder."

You should see `grocery-list.txt` and `notes.txt`. Then ask:

> "Read my grocery list."

The server reads the file on your computer and hands the text to the AI. Your file never left your machine.

## If something does not work

| Problem | What to try |
|---------|-------------|
| `npx: command not found` | Install Node.js from nodejs.org, then open a new terminal window |
| Server says "folder not found" | Double-check the path to your `mcp-practice` folder |
| AI client cannot find the server | Restart the AI client and re-check the server settings |

## Glossary

- **Terminal**: The app where you type commands to your computer.
- **npx**: A tool that downloads and runs a program without installing it permanently.
- **stdio server**: An MCP server that runs on your computer and exchanges text with your AI client.
- **Arguments**: The extra pieces of text you pass to a command (like the folder path).

---

*Next: [Safety rules for file access](04-safety-rules-for-file-access.md)*

*Published by Asdale Dynamics, LLC — beginner-friendly AI education, books, and tools.*
