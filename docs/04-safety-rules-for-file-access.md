# Safety Rules for File Access

Giving an AI access to your files is convenient, but it is also a power you should hand out carefully. These rules are written for beginners. Follow them every time you connect an MCP server to your computer.

## Rule 1: Start with one small folder

Never point a new MCP server at your whole computer, your Documents folder, or your desktop on the first try. Create one practice folder, put harmless files in it, and let the server see only that folder. Once you trust the server, you can decide whether to give it more.

## Rule 2: Know what the server can reach

Before you run any MCP server, ask:

- Which folders can it read?
- Can it write, edit, or delete files, or only read them?
- Can it reach files outside the folder I chose?

If you cannot answer these questions, do not run the server yet.

## Rule 3: Run servers on your own computer

Prefer stdio servers that run locally. Your files stay on your machine, and nothing is uploaded unless you choose to share it. Be cautious with servers that require you to create an account, enter an API key, or send your files to a website you do not recognize.

## Rule 4: Never put secrets in files the server can see

Passwords, API keys, credit card numbers, Social Security numbers, and medical records do not belong in a folder an AI can read. If a file contains secrets, keep it outside any MCP-connected folder.

## Rule 5: Approve important actions

A good setup asks you before sending email, deleting files, or spending money. If an agent offers to do something important without asking you first, say no and check its settings.

## Rule 6: Know who made the server

Only run MCP servers from people or companies you trust. An MCP server is a program that runs on your computer, so it deserves the same caution as any other program you download.

## Rule 7: You are always in charge

You can stop an MCP server at any time. You can remove its access to a folder. You can delete the practice folder and start over. If something feels wrong, turn it off.

## Quick safety checklist

Run through this before connecting any new server:

- [ ] I know which folder this server can reach, and it is not my whole computer
- [ ] The folder contains no passwords, API keys, or personal documents I want to keep private
- [ ] The server runs on my computer (stdio), not on a website I do not recognize
- [ ] I know who made the server and I trust them
- [ ] The AI client will ask me before sending email or deleting files
- [ ] I know how to stop the server and remove its access

## If something goes wrong

- Stop the server in your AI client's settings
- Delete or move the practice folder
- Change any password or API key that might have been exposed
- Ask a more experienced friend for help, or contact Asdale Dynamics, LLC through dylanasdale.github.io

---

*Published by Asdale Dynamics, LLC — beginner-friendly AI education, books, and tools.*
