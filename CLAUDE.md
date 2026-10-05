# Standing instructions for this project

Claude Code reads this file at the start of every session in this folder. The line below loads the memory index at the same time.

This file is built on the way Boris Cherny, who created Claude Code, says he and his team work: one CLAUDE.md kept in the project, a line added every time Claude gets something wrong, a plan agreed before anything is built, and a way for Claude to check its own work.

@memory/MEMORY.md

## About me

- I am a lawyer and I do not write code. Use plain English and short sentences, and define each technical term the first time you use it.
- When I need to do something (click, sign in, approve), give me numbered steps.
- If you are unsure what I want, ask one question before you start.
- I will ask questions about anything I do not understand: the tools, the steps, an error message, or what you are doing. Answer them plainly and patiently, as many times as I need.

## Confidentiality: fictional data only

- Use fictional data only, in every file, including the memory folder. Do not ask for, use or store real client names, matters, documents or personal information.
- Make up example data with clearly fictional names, such as "Northwind Trading Pty Ltd" or "Jane Example".
- If I paste something that looks like real client information, stop, tell me, and do not save it to any file.
- The memory folder is saved to GitHub with the rest of the project. Write every note so that it is safe for someone else to read.

## Project memory

- The project memory is the `memory/` folder. Its index is `memory/MEMORY.md`, loaded above.
- A link written [[name]] means the file `memory/name.md`. A link written [[decisions/name]] means `memory/decisions/name.md`.
- Record project facts and decisions in the memory folder rather than in your own auto memory, so that I can read them in Obsidian and they are saved to GitHub.
- At the start of every session, read the index, the latest session log in `memory/sessions/`, and the notes the task needs. Read [[problem]] and [[redesign]] before you work on the tool itself.
- Before you act on anything that depends on an earlier decision, open the decision note and name it, for example "Following [[decisions/2026-10-17-sort-by-due-date]]".
- If two notes disagree, tell me which notes and ask which one is correct.
- If neither the memory nor the project files answer a question, say so and ask me. Do not guess. Do not invent facts, names, laws, figures, case names or citations.
- When we decide something, write a decision note in `memory/decisions/` in the format set out in [[decisions/README]]. Add one line for it to the index and link it to the related notes.
- Record where each fact came from in [[sources]], and put the source number after the fact in the note, for example "(S3)". Mark a fact with no known source "(source unknown)".
- At the end of every session, or when I say we are stopping, write a session log in `memory/sessions/` in the format set out in [[sessions/README]]: what was done, what changed, what is next. Then update the index.
- Each note starts with a header block: a title line, then type (problem, redesign, decision, source, session, glossary or guide), date, and related links.
- Keep notes short. To change a fact, edit the note that holds it and update its date; do not start a second note on the same topic.
- To change a decision, write a new decision note and mark the old one "replaced by" the new one. Keep the old note.
- Keep the index to one line per note: `- [[note-name]] - one-line summary`.
- You may write memory notes without asking first. At the end of your reply, list the notes you created or changed.

## Plan first

- For anything bigger than a small fix, write a short plan before you build: what you will change, in which files, and how we will check it works. Go back and forth with me until I agree the plan. Only then start.
- If the plan changes while you are building, stop and tell me.

## Before you change anything else

- Before you create, edit or move any other file, tell me in two or three plain sentences what you plan to change and why. Wait for me to agree.
- Keep each change small: one feature or one fix at a time.
- Ask before deleting any file, folder, note or data. Say what will be lost and wait for a clear yes.

## Check your own work

- Before you tell me something is done, check it yourself: run it, open it, or try it with a fictional example, and tell me what you saw.
- If you could not check it, say so plainly and tell me how I can check it.
- After each change, tell me which files changed and the one thing I should try to confirm it works.

## Saving work to GitHub

- Save to GitHub only when I ask. Then commit the changes with a one-line message in plain English that says what changed, and push them to GitHub.
- Before each save, check that no file contains client information, passwords, recovery codes or keys. Keep secret files (such as .env) out of GitHub by listing them in .gitignore.
- If a save fails, explain the error in plain English and suggest one fix. Ask before changing any GitHub setting.

## Lessons

Every time Claude gets something wrong, or I have to repeat an instruction, add one line here so it does not happen again. Ask me before adding it.

- (No lessons yet.)

## Where this structure comes from

- Boris Cherny, creator of Claude Code, on how his team works (2 January 2026): keep one CLAUDE.md in the project and add to it "Anytime we see Claude do something incorrectly"; start in Plan mode and agree the plan first; give Claude a way to verify its work.
- Anthropic's guidance on CLAUDE.md files: code.claude.com/docs/en/memory.
- The memory folder (an index with one line per note, plus one note per topic) follows the layout of Claude Code's own auto memory.
