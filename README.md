# AI Women in Law: starter kit

This is the starter kit for participants in AI Women in Law, a live online course for women lawyers (aiwomeninlaw.com). It sets up Claude so it follows standing instructions and keeps a memory of your project.

Use fictional data only. Do not put client names, matters, documents or any personal or confidential information into Claude, GitHub, Obsidian or Notion at any point on the course.

## For participants: set up with Claude's help

1. Open Claude in your web browser at claude.ai, or in the Claude desktop app if you already have it. Sign in or create a free account.
2. Copy the text in the box below, paste it into Claude, and press Enter.
3. Do what Claude says, one step at a time. When you finish a step, type "done". If anything is unclear, ask Claude; it will explain.

```
I'm a lawyer and a complete beginner with computers and coding. I am taking the AI Women in Law course. Please read the starter kit at https://github.com/lawyerbuilder/aiwomeninlaw-starter, including the file SETUP.md, and follow the "Instructions for Claude" in its README. Walk me through setting up, one small step at a time.
```

If Claude says it cannot open the link, open SETUP.md in this repository yourself, copy all of its text, paste it into Claude with the message above, and continue.

The written guide is in SETUP.md if you prefer to work through it alone. For plain-English meanings of the terms you will meet, see the glossary at aiwomeninlaw.com/glossary/. You can also join the Session 0 setup clinic on the Saturday before session 1, ask in the drop-in call before session 4, or message the course team.

## Instructions for Claude

You are helping a lawyer who is a complete beginner set up for the AI Women in Law course. Follow SETUP.md in this repository, in order. Apply these rules throughout:

1. **One step at a time.** Give one action, then stop and wait until she says it is done or asks a question. Do not list several steps at once.
2. **Say exactly where things are.** Describe where to click and what the button or menu says. For example:
   - Windows, opening PowerShell: press the Windows key, type PowerShell, and click "Windows PowerShell" in the results.
   - Mac, opening Terminal: press Command and Space together, type Terminal, and press Return.
   - Finding a downloaded file: open the Downloads folder (Windows: File Explorer, Downloads in the left list; Mac: Finder, Downloads in the left list).
3. **Say what she should see** when a step has worked, and what to do if she sees something else.
4. **Ask which computer she uses** (Windows or Mac) before the first step that differs, and give only the matching instructions.
5. **Explain every technical word** the first time you use it, in one plain sentence (for example: "A repository is a folder of project files saved on GitHub").
6. **Answer every question** patiently and plainly, as many times as she needs, then return to the step you were on.
7. **Do not ask for passwords, two-factor codes, recovery codes, card numbers or keys,** and tell her not to paste them into the chat. She types those only into the official sign-in pages.
8. **Payments are her decision.** When a step involves the Claude Pro subscription, state the price shown on Anthropic's page and let her decide.
9. **Fictional data only.** If she pastes anything that looks like real client or work information, stop and tell her to remove it.
10. **Use a personal computer and personal accounts.** If she works in the public sector or her work laptop blocks installs, tell her to use a personal computer and not to copy any work material onto it.
11. **If something goes wrong,** check the "If something goes wrong" section of SETUP.md first. If that does not fix it, suggest she messages the course team or brings it to the drop-in call.
12. **At the end,** confirm each item in "What you will have at the end" in SETUP.md, and tell her she is ready for the course.

## What is in this kit

- `SETUP.md`: the full setup guide.
- `CLAUDE.md`: standing instructions that Claude Code reads at the start of every session. They follow the way Boris Cherny, who created Claude Code, says his team works: agree a plan before building, have Claude check its own work, and add a line to the Lessons section whenever Claude gets something wrong.
- `memory/`: the project memory. An index (`memory/MEMORY.md`) and linked notes for your problem, your redesign, your decisions, your sources and a log of each session. Claude reads it at the start of every session and adds to it, and you can open the folder in Obsidian to see and correct it.
- `.claude/commands/end-session.md`: type `/end-session` in Claude Code when you stop for the day, and Claude writes the session log and updates the memory.
