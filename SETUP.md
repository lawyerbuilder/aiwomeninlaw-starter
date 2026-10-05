# AI Women in Law: setup guide

This guide is for participants who prefer to set up on their own instead of attending the optional Session 0 setup clinic. It covers the same steps as the clinic. Instructions were checked against the vendors' own pages on 5 October 2026. The vendors change their screens from time to time, so a button label may differ slightly from the wording here.


**If you have a question at any step, ask Claude.** Once Claude is installed (Part 1), you can type any question into it, such as "What is a repository?" or "I see this error, what does it mean?", and it will explain. You can also ask Claude to walk you through this whole guide: see "Set up with Claude's help" at aiwomeninlaw.com/setup/.

## What you will have at the end

1. A Claude Pro account and the Claude desktop app, with Claude Code open in the Code tab.
2. A project folder called my-first-tool that holds your standing instructions (CLAUDE.md) and your project memory (the memory folder), saved to a private GitHub repository.
3. Obsidian, a free notes app, open on your memory folder so you can read and correct what Claude has written down.
4. A Vercel account on the free Hobby plan, ready for the optional clinic after session 5, where you publish your tool.
5. Optional: a Notion connection, so Claude can write a weekly summary page for your buddy or manager.

**How long it takes:** 75 to 105 minutes, plus download time. You can stop at the end of any part and continue later.

## Before you start

You need:

1. **A computer you can install software on.** Windows 10 or 11, or a Mac on macOS 13 (Ventura) or later. If your work laptop blocks installs, use a personal computer for the whole course.
2. **An email address** that you will keep using for the course. A personal address is simplest.
3. **A mobile phone** for two-factor authentication codes, with an authenticator app installed (for example Google Authenticator or Microsoft Authenticator).
4. **A payment card** for the Claude Pro subscription.

**Confidentiality.** Do not paste client information into Claude, GitHub, Vercel, Obsidian or Notion at any point on this course. Use fictional names, matters and documents in every prompt, file, note and example. This applies to your own employer's information too.

---

## Part 1: Claude

### Create your account

1. In your web browser, go to **claude.ai**.
   You should see a sign-in page with a box for your email address and a **Continue with Google** button.
2. Enter your email address and click **Continue with email**, or click **Continue with Google**.
   With email, you should see a message that a sign-in link has been sent.
3. Open the email from Claude and click the sign-in link (skip this step if you used Google).
   You should see the Claude chat screen in your browser.

### Choose the Pro plan

On 5 October 2026 the Claude pricing page (claude.com/pricing) showed Pro at **US$20 per month** billed monthly, or **US$17 per month** with annual billing (US$200 paid up front). Prices exclude tax, and Claude charges in your local currency where it supports one. Check the pricing page for your current price before you subscribe. Claude Code is included in Pro. The free plan does not include Claude Code.

4. Click your initials or name in the lower left corner, then click **Settings**.
   You should see the Settings page.
5. Click **Billing**, then click **Upgrade plan**.
   You should see the plan options.
6. Click **Get Pro plan**.
   You should see a choice between monthly and annual billing.
7. Choose **monthly** or **annual**.
   You should see the payment form.
8. Enter your card details and click **Subscribe**.
   You should see a confirmation, and **Settings > Billing** now shows the Pro plan.

### Install the Claude desktop app

9. Go to **claude.com/download**.
   You should see download buttons for macOS and Windows.
10. Download the version for your computer:
    - **Mac:** click **Download for macOS**.
    - **Windows:** most laptops need the standard Windows download. If your laptop has an ARM processor, choose **Windows (arm 64)** instead. To check, open **Settings > System > About** and read **System type**: "x64-based processor" means the standard download, "ARM-based processor" means arm 64.

    You should see the installer file in your Downloads folder.
11. Open the installer file.
    - **Mac:** a window opens with the Claude icon. Drag the Claude icon into the **Applications** folder.
    - **Windows:** the installer runs and Claude opens when it finishes.
12. Open Claude: from the **Applications** folder on a Mac, or from the **Start** menu on Windows.
    You should see a sign-in screen.
13. Sign in with the same email address or Google account you used in step 2.
    You should see the Claude app with three tabs at the top: **Chat**, **Cowork** and **Code**.
14. Click the **Code** tab.
    You should see a prompt box with a folder selector. If you see a message asking you to upgrade, your Pro subscription has not started yet: repeat steps 4 to 8.

The Code tab includes Claude Code. You do not need to install anything else for Claude Code, and you do not need to use a terminal for it.

---

## Part 2: GitHub

GitHub stores a copy of your project online and keeps every saved version, so you can go back to an earlier version if a change goes wrong. A free personal account is enough for the course.

### Create your account

1. Go to **github.com/signup**.
   You should see the sign-up form, with an option to **Continue with Google**.
2. Enter your email address, a password and a username, and choose your country. Choose a username you are happy for others to see, because it appears in the web address of your projects.
   You should see a verification puzzle or a request for a code.
3. Complete the verification puzzle if GitHub shows one.
4. Open the email from GitHub and enter the code it contains (or click the verification link).
   You should see your GitHub home page, with your profile picture in the upper right corner.

### Turn on two-factor authentication

Two-factor authentication means GitHub asks for a code from your phone each time you sign in on a new device. GitHub requires it for accounts that contribute code, and gives a set period to turn it on. Turn it on now so it does not interrupt you during a session. GitHub recommends an authenticator app over text messages.

5. Click your profile picture (upper right), then **Settings**.
   You should see your account settings.
6. In the left menu, under **Access**, click **Password and authentication**.
   You should see a **Two-factor authentication** section.
7. Click **Enable two-factor authentication**.
   You should see a QR code under **Scan the QR code**.
8. On your phone, open your authenticator app, add a new account, and scan the QR code.
   You should see a new GitHub entry in the app showing a six-digit code that changes every 30 seconds.
9. Type the current six-digit code into the box on the GitHub page.
   You should see your recovery codes.
10. Click **Download** and save the recovery codes file somewhere safe outside your project folder, for example your password manager or a printed copy kept at home.
    You should see the file in your Downloads folder.
11. Click **I have saved my recovery codes**.
    You should see a message that two-factor authentication is enabled.

The recovery codes let you into your account if you lose your phone. Keep them out of the my-first-tool folder, because everything in that folder is saved to GitHub.

---

## Part 3: Claude Code and your project memory

Each Claude Code session starts as a new conversation: Claude does not see what was said in earlier sessions unless it was written to a file. The course gives your project a memory folder so that what you decide in week 1 is still written down in week 4. The course calls this folder your **memory palace**: a set of short notes, linked to each other, that Claude reads at the start of every session and updates as you work. Each note covers one subject: the problem, the redesign, one decision, one session, the sources of your facts, and a glossary.

The starter kit has two parts:

- **CLAUDE.md**, your standing instructions. Claude Code reads this file at the start of every session in the folder. Its line `@memory/MEMORY.md` tells Claude Code to load the memory index at the same time. CLAUDE.md also tells Claude to read the notes a task needs, to name the decision note it is relying on, to write down each new decision and where each fact came from, to write a session log at the end of each session, and to say so and ask you when something is missing, instead of guessing. It is built on how Boris Cherny, who created Claude Code, works: agree a plan before building, have Claude check its own work, and add a line to the Lessons section of CLAUDE.md each time Claude gets something wrong.
- **.claude/commands/end-session.md**, a shortcut. When you stop for the day, type `/end-session` in the prompt box. Claude writes the session log, files any missing decision notes, updates the index and suggests a line for Lessons.
- **The memory folder.** MEMORY.md is the index, with one line per note. The other notes start almost empty, with headings and one-line instructions, and fill up as you work.

Claude Code also keeps notes of its own, called auto memory, in a folder outside your project. The course relies on the memory folder instead, because you can read it in Obsidian, correct it, and save it to GitHub with the rest of the project. CLAUDE.md tells Claude to record project facts in the memory folder.

### Make the folder and add the starter files

1. Create a new folder called **my-first-tool** in your Documents folder.
   - **Windows:** open **File Explorer**, click **Documents**, then **New > Folder**, and type `my-first-tool`.
   - **Mac:** open **Finder**, click **Documents**, then **File > New Folder**, and type `my-first-tool`.

   You should see an empty folder called my-first-tool.
2. Download the starter kit from https://github.com/lawyerbuilder/aiwomeninlaw-starter/archive/refs/heads/main.zip (or open github.com/lawyerbuilder/aiwomeninlaw-starter and click **Code**, then **Download ZIP**).
   You should see a file called aiwomeninlaw-starter-main.zip in your Downloads folder.
3. Unzip the file.
   - **Windows:** right-click aiwomeninlaw-starter-main.zip, click **Extract All**, then click **Extract**.
   - **Mac:** double-click aiwomeninlaw-starter-main.zip.

   You should see a folder called **aiwomeninlaw-starter-main** in your Downloads folder.
4. Open that folder, select **CLAUDE.md**, the **memory** folder and the **.claude** folder, and copy them into my-first-tool. (On a Mac, press Command, Shift and full stop together to show the .claude folder, which is hidden by default. On Windows, in File Explorer click **View**, then **Show**, then **Hidden items**.)
   You should see three items in my-first-tool: the file CLAUDE.md and the folders memory and .claude.
5. Open the memory folder.
   You should see five files (MEMORY.md, problem.md, redesign.md, sources.md, glossary.md) and two folders (decisions and sessions). Each of the two folders holds one file, README.md, which explains how to write a decision note or a session log.

You can delete the aiwomeninlaw-starter-main folder and the zip file from your Downloads folder now. Keeping a second copy makes it easy to open the wrong one later.

### Open the folder in Claude Code

6. In the Claude app, click the **Code** tab.
   You should see the prompt box with options below or beside it.
7. Choose **Local** as the environment.
   Local means Claude works on the files on your own computer.
8. Click **Select folder** and choose **my-first-tool** in your Documents folder.
   You should see "my-first-tool" shown as the selected folder.
9. Click the permission mode selector next to the send button and choose **Manual**.
   Manual means Claude asks before it edits a file or runs a command, and shows you the change first. (Older versions of the app call this mode **Ask permissions**.)

### Check that Claude has read the memory

10. Copy this prompt into the prompt box and press **Enter**:

```text
Please check that you have read the project memory. Do not change any files.
1. List each note in the memory index (memory/MEMORY.md) with its one-line summary.
2. Open memory/problem.md and memory/redesign.md and list their headings.
3. In no more than six bullet points, tell me what CLAUDE.md asks you to do with the memory folder.
4. Tell me what you will do if I ask about something that is in neither the memory folder nor the project files.
```

You should see:

- six notes listed: problem, redesign, glossary, sources, decisions/README and sessions/README;
- the headings of the problem and redesign notes, with a remark that they are not filled in yet;
- bullet points that mention reading the index at the start of a session, writing decision notes, recording sources, and writing a session log;
- an answer to question 4 saying that Claude will tell you the information is missing and ask you, instead of guessing.

If Claude asks permission to read the files, approve it. If Claude does not list the notes, see "Claude did not read the memory" under **If something goes wrong**.

---

## Part 4: Open your memory in Obsidian

Obsidian is a notes app that reads and edits ordinary Markdown (.md) files in a folder on your computer. Obsidian calls such a folder a **vault**. You will open your memory folder as a vault, so you can read Claude's notes, follow the links between them, and correct a note when it is wrong.

On 5 October 2026 the Obsidian licence page stated that Obsidian is free for all purposes, including personal and commercial use, and that the commercial licence is optional. You do not need an Obsidian account or any paid add-on for this course.

### Install Obsidian

1. Go to **obsidian.md/download**.
   You should see download options for Windows and macOS.
2. Download the version for your computer:
   - **Windows:** click **Download for Windows**.
   - **Mac:** click the **Universal** download (a .dmg file).

   You should see the installer file in your Downloads folder.
3. Open the installer file.
   - **Windows:** the installer runs and Obsidian opens when it finishes.
   - **Mac:** a window opens with the Obsidian icon. Drag it into the **Applications** folder, then open Obsidian from **Applications**.

   You should see the Obsidian start screen, with options that include **Create new vault** and **Open folder as vault**.

### Open the memory folder as a vault

4. Next to **Open folder as vault**, click **Open**.
   You should see a window for choosing a folder.
5. Go to **Documents**, open **my-first-tool**, click the **memory** folder once to select it, and click **Open** (on Windows the button may say **Select Folder**).
   You should see the Obsidian main window. The list on the left shows MEMORY, problem, redesign, sources and glossary, and the folders decisions and sessions.
6. If Obsidian asks whether you trust the author of this vault, click **Browse vault in Restricted Mode**.
   Restricted Mode turns off add-ons written by other people. The course does not use them.

Choose the memory folder, and avoid choosing my-first-tool. The links in your notes are written from the memory folder, so they only work when memory is the vault.

Obsidian adds a hidden folder called .obsidian inside memory for its own settings. Leave it there. Part 5 keeps it out of GitHub.

### Read the notes and see the links

7. In the list on the left, click **MEMORY**.
   You should see the index. Each note name appears as a link, in a different colour from the text around it.
8. Click the link **problem**.
   You should see the problem note open, with its headings and one-line instructions.
9. In the narrow column of icons at the far left (Obsidian calls it the ribbon), click **Open graph view**.
   You should see a circle for each note and a line between each pair of notes that link to each other. MEMORY is joined to every other note.
10. Click the **problem** tab at the top of the window to go back to the problem note. In the right sidebar, click the **Backlinks** tab.
    You should see **Linked mentions**, listing the notes that link to problem, including MEMORY and redesign. If you cannot see the Backlinks tab, press **Ctrl+P** (Windows) or **Cmd+P** (Mac), type `Backlinks: Show backlinks`, and press **Enter**.

As you build, Claude adds decision notes and session logs. Each one appears in the list on the left and as a new circle in the graph view, joined to the notes it links to.

### Correct a note

When a note says something wrong, correct it yourself and then tell Claude, so that the correction is recorded and Claude works from the corrected version.

11. In Obsidian, open the note and click into the text you want to change.
12. Type the correction, and change the date in the header block at the top of the note to today's date.
    Obsidian saves the change automatically after a couple of seconds.
13. At the start of your next Claude Code session, tell Claude what you changed. For example:

```text
I corrected memory/problem.md: the review step takes three days, and the note said one day. I took the figure from the team's fictional review log. Please read the note again, add the source to memory/sources.md, and check whether any other note relies on the old figure.
```

   You should see Claude read the note, propose an entry for sources.md, and list any other notes that mention the old figure.

To change a decision, ask Claude to write a new decision note and mark the old one as replaced. The old note stays in the folder, so you can see what was decided before and why it changed.

---

## Part 5: Connect GitHub so Claude Code can save your work

Claude Code saves your work to GitHub with two free programs: **Git**, which records versions of your files, and **GitHub CLI**, which signs your computer in to your GitHub account. You install both once, then sign in once.

### Install Git

1. Install Git:
   - **Windows:** go to **git-scm.com/install/windows** and download the standalone installer for your computer (x64 for most laptops, ARM64 for ARM laptops). Open the file and click **Next** on each screen without changing the options, then **Install**, then **Finish**.
   - **Mac:** open **Terminal** (press Cmd+Space, type Terminal, press Enter). Copy this line into the Terminal window and press Enter:

```text
git --version
```

   - **Windows:** you should see **Git Bash** in your Start menu.
   - **Mac:** you should see a line such as "git version 2.x". If instead a window offers to install the "command line developer tools", click **Install**, accept the licence, wait for it to finish, and run the line again.

### Install GitHub CLI

2. Go to **github.com/cli/cli/releases/latest** and scroll to **Assets**.
   You should see a list of files whose names start with "gh_".
3. Download the installer for your computer:
   - **Windows:** the file ending **windows_amd64.msi** (or **windows_arm64.msi** on an ARM laptop).
   - **Mac:** the file ending **macOS_universal.pkg**.

   You should see the file in your Downloads folder.
4. Open the file and follow the installer, keeping the default options.
   You should see a message that the installation succeeded.
5. Restart your computer.
   This makes sure the Claude app can find the two new programs.

### Sign in to GitHub from Claude Code

6. Open the Claude app, click the **Code** tab, and open your my-first-tool session from the sidebar (or start a new Local session on the my-first-tool folder).
   You should see your earlier conversation, or an empty session with my-first-tool selected.
7. Press **Ctrl+`** (the Ctrl key and the backtick key, usually below Esc). This uses Ctrl on Mac as well as Windows.
   You should see a terminal pane open inside the app.
8. Copy this line into the terminal pane and press **Enter**:

```text
gh auth login --hostname github.com --git-protocol https --web
```

   You should see the question "Authenticate Git with your GitHub credentials? (Y/n)".
9. Press **Enter** to answer yes.
   You should see "First copy your one-time code:" followed by a code in the form XXXX-XXXX.
10. Write down the code, then press **Enter**.
    You should see your browser open at a GitHub device activation page.
11. Sign in to GitHub if asked (with your password and a code from your authenticator app), type the code from step 10, and click **Continue**.
    You should see a page asking you to authorise GitHub CLI.
12. Click **Authorize github**.
    You should see a message in the browser that the device is connected, and in the terminal pane: "Authentication complete" and "Logged in as" followed by your GitHub username.

### Make your first save

13. Click back into the prompt box (outside the terminal pane), copy this prompt and press **Enter**:

```text
Please save this project to GitHub for the first time.
1. Set this folder up as a Git repository if it has not been set up already.
2. If Git does not yet have a name and email for me, use my GitHub username as the name and my GitHub no-reply email address as the email. Look both up with the GitHub CLI.
3. Create a file called .gitignore that lists .env and memory/.obsidian/, so that those stay on this computer.
4. Check that no file contains client information, passwords, recovery codes or keys.
5. Write today's session log in memory/sessions/, following memory/sessions/README.md. What was done: "Project set up; starter files saved to GitHub." Add the log to the index in memory/MEMORY.md.
6. Create a private repository called my-first-tool on my GitHub account and save (commit and push) all the files to it, with the message "Starter files: CLAUDE.md and memory folder".
7. Tell me the web address of the repository.
```

   You should see Claude describe each step and ask your permission before each command. Read the one-line description of each command and approve it.
14. When Claude gives you the web address, open it in your browser.
    You should see your repository page on GitHub, marked **Private**, listing .gitignore, CLAUDE.md and the memory folder.
15. In Obsidian, click the **sessions** folder in the list on the left.
    You should see today's session log next to README.

From now on, when you want to save your work, ask Claude in plain words, for example "Please save my work to GitHub with a message that says what changed." The memory folder is saved with the rest of the project, so treat every note as something another person could read.

---

## Part 6: Vercel

Vercel publishes your tool on the internet. In this part you only create the account. Publishing comes in the optional clinic after session 5.

The Hobby plan is free. Vercel's terms limit Hobby to personal or non-commercial use. A course project built with fictional data is a personal project. If your tool later goes into use at your firm or organisation, Vercel requires a paid plan for that, so check the Vercel fair use guidelines at that point.

1. Go to **vercel.com/signup**.
   You should see sign-up buttons including **Continue with GitHub**.
2. Click **Continue with GitHub**.
   You should see a GitHub page asking you to authorise Vercel. Sign in to GitHub first if asked.
3. Click **Authorize Vercel**.
   You should return to Vercel.
4. If Vercel asks which plan or what you are working on, choose **Hobby** (personal projects) and enter your name.
5. If Vercel offers to import a Git repository or start from a template, leave it for now and go to your dashboard.
   You should see your Vercel dashboard with your name or username in the upper left corner.

Setup is complete. Part 7 is optional.

---

## Part 7 (optional): Connect Notion

Notion is an online notes app. If your course buddy or your manager would like a short weekly update, Claude can write it as a page in your own Notion workspace, using what is in your memory folder. The memory folder stays the record: Claude writes the Notion page from the memory folder, and Claude does not copy changes you make in Notion back into the memory folder. If a fact is wrong, correct it in the memory folder (Part 4, steps 11 to 13).

You need a Notion account. If you do not have one, create it at notion.com before you start this part.

**Check which workspace you connect.** Notion states that the connection acts with your full Notion permissions, so Claude can read and change any page you can. Connect a personal Notion workspace, and avoid connecting a workspace that belongs to your employer. The fictional-data rule applies to Notion pages too.

### Add the Notion connector

1. In the Claude app, click **Customize** in the sidebar, then click **Connectors**.
   You should see the connectors you have added, which may be none.
2. Click the **+** button next to **Connectors**, then click **Browse connectors**.
   You should see a directory of connectors.
3. Find **Notion** (made by Notion) and click **Connect**.
   You should see a Notion page in your browser asking you to sign in.
4. Sign in to Notion, choose your personal workspace, and allow access.
   You should return to the Claude app, with Notion listed under **Connectors**.
5. Click the **Code** tab and open your my-first-tool session. Click the **+** button next to the prompt box, then click **Connectors**.
   You should see Notion in the list, switched on. If it is switched off, click it to switch it on.

### Write a weekly summary

6. Copy this prompt into the prompt box and press **Enter**:

```text
Please write this week's summary for my course buddy.
1. Read memory/MEMORY.md, the session logs in memory/sessions/ from the last seven days, and any decision notes dated in the last seven days.
2. Draft the summary in plain English, in no more than 300 words, under three headings: What I built, What I decided (one line per decision, with the decision note's name), What is next.
3. Use only what is in the memory folder. If something is missing, say so in the draft instead of filling the gap.
4. Show me the draft and wait for my approval before you write anything to Notion.
5. After I approve, create a new private page in my Notion workspace titled "My first tool: week of" followed by today's date, containing the summary. Give me the link to the page.
6. Do not read, change or move any other Notion page.
```

   You should see the draft in the Code tab, and no change in Notion yet.
7. Read the draft. If it is right, reply "Approved". If something is wrong, say what to change, and correct the memory note first if the mistake comes from there.
   You should see Claude ask permission to use the Notion connector. Approve it.
8. Open the link Claude gives you.
   You should see the new page in your Notion workspace with the three headings.

To share the page, use the **Share** button in Notion and add your buddy's or manager's email address.

---

## If something goes wrong

1. **Your work laptop blocks an install, or Local is greyed out in the Code tab.**
   Your organisation's settings prevent it. Use a personal computer for the course, and start again from Part 1, step 9 on that computer. Your accounts stay the same.

2. **The Code tab asks you to upgrade, or shows "Error 403".**
   Check that **Settings > Billing** shows the Pro plan. Then sign out of the Claude app and sign in again. If that does not fix it, restart the computer (closing the app window leaves it running), then open the app and sign in.

3. **GitHub rejects the two-factor code, or the code does not arrive.**
   Authenticator app codes depend on your phone's clock: set the phone's date and time to update automatically, then use a fresh code. If you chose text messages and the code does not arrive, switch to an authenticator app; GitHub states that text message delivery is unreliable and is unavailable in some countries. If you cannot sign in at all, use one of your recovery codes.

4. **Claude says it cannot find CLAUDE.md or memory/MEMORY.md.**
   Check the file names. Windows hides file extensions by default, so a file may really be called CLAUDE.md.txt. In File Explorer, click **View > Show > File name extensions**, then rename the file so it ends in .md. Check that CLAUDE.md and the memory folder sit directly inside my-first-tool, and that they are not inside a starter folder within it.

5. **Claude did not read the memory.** For example, Claude cannot list your notes, or asks what the project is about.
   - Check that CLAUDE.md contains the line `@memory/MEMORY.md` on a line of its own, with nothing before the @ sign.
   - Check that the folder is called memory (all lower case) and that MEMORY.md is directly inside it.
   - Start a new session (**+ New session** in the sidebar, then **Local** and **Select folder** > my-first-tool). Claude Code loads CLAUDE.md and the index when a session starts, so a change made during a session takes effect in the next one.
   - Type `/context` in the prompt box and press **Enter**. Under **Memory files** you should see CLAUDE.md and memory/MEMORY.md. If the command is unavailable in your version of the app, ask Claude: "Please read memory/MEMORY.md and list the notes in it."

6. **A note is wrong.**
   Correct it in Obsidian and tell Claude at the start of the next session (Part 4, steps 11 to 13). If Claude wrote the wrong fact because it guessed, add a line to CLAUDE.md under **Project memory** that names the mistake, for example "Do not state turnaround times unless a note gives one." If two notes disagree, ask Claude to list both and tell it which one is right, then ask it to correct the other note and update the index.

7. **Obsidian shows a different folder, or notes Claude says it wrote are missing.**
   Look at the vault name at the bottom of the left sidebar: it should say memory. If it shows another name, click it, click **Manage vaults**, click **Open** next to **Open folder as vault**, and choose Documents > my-first-tool > memory. If the vault name is memory and notes are still missing, you may have opened a second copy of the folder (for example the starter folder in Downloads); delete that copy and open the one in my-first-tool.

8. **Claude is working in the wrong folder.**
   Look at the folder name shown next to the prompt box. Start a new session (**+ New session** in the sidebar), choose **Local**, click **Select folder**, and choose my-first-tool.

9. **The computer does not recognise "gh" or "git", or the installer will not open.**
   Restart the computer and try again, because new programs are only found after a restart. If your Mac says it cannot verify the GitHub CLI installer, leave your security settings as they are and message the team (see below); we will walk you through it.

10. **The first save fails with "Authentication failed" or "Permission denied".**
    In the terminal pane (Ctrl+`), run the line below. If it does not say "Logged in to github.com", repeat Part 5, steps 8 to 12.

```text
gh auth status
```

11. **Claude asks a question you do not understand.**
    Ask Claude to explain it in plain English before you approve anything. You can also choose **Reject** (or the equivalent button) on any change, and Claude will ask how you want to proceed.

## Where to get help

1. **The Session 0 setup clinic recording.** It shows every step in this guide on screen. [Recording link to be confirmed.]
2. **The drop-in call before session 4**, for anyone still stuck on setup. [Date and link to be confirmed.]
3. **Message the team** in your cohort group, or by email at [course email to be confirmed]. Say which part and step number you reached, and attach a screenshot. Do not include passwords, recovery codes or any client information in a message or screenshot.

---

## Screenshots to capture (facilitator checklist)

Capture each on both Windows and Mac where the screen differs. Hide email addresses, card details, recovery codes and one-time codes before adding them.

1. Part 1, step 2: claude.ai sign-in page.
2. Part 1, step 5: Settings > Billing with the Upgrade plan button.
3. Part 1, step 6: plan options with Get Pro plan.
4. Part 1, step 10: claude.com/download buttons (Mac, Windows, Windows arm 64).
5. Part 1, step 10: Windows Settings > System > About showing System type.
6. Part 1, step 11: Mac installer window with the Applications folder.
7. Part 1, step 13: Claude app showing the Chat, Cowork and Code tabs.
8. Part 2, step 2: GitHub sign-up form.
9. Part 2, step 6: GitHub Settings > Password and authentication.
10. Part 2, step 7: the QR code screen (QR code blurred).
11. Part 2, step 9: recovery codes screen with Download (codes blurred).
12. Part 3, step 3: Windows Extract All dialog for aiwomeninlaw-starter-main.zip.
13. Part 3, step 4: my-first-tool containing CLAUDE.md and the memory folder (Windows with extensions shown).
14. Part 3, step 5: the memory folder contents (five files, two folders).
15. Part 3, steps 7 to 9: Code tab with Local, Select folder and the Manual permission mode visible.
16. Part 3, step 10: Claude's reply listing the six notes and answering question 4.
17. Part 4, step 2: obsidian.md/download with the Windows and Universal (Mac) downloads.
18. Part 4, step 3: Obsidian start screen with Open folder as vault.
19. Part 4, step 5: folder picker with the memory folder selected (Windows Select Folder, Mac Open).
20. Part 4, step 6: the trust prompt with Browse vault in Restricted Mode (if shown).
21. Part 4, step 7: the MEMORY index open, with links visible.
22. Part 4, step 9: graph view with the ribbon icon highlighted.
23. Part 4, step 10: Backlinks tab showing Linked mentions for problem.
24. Part 4, step 12: a note being edited, with the header block date changed.
25. Part 5, step 1: Git for Windows installer first screen; Mac command line developer tools pop-up.
26. Part 5, step 2: GitHub CLI release page with the Assets list.
27. Part 5, step 7: terminal pane open in the Code tab.
28. Part 5, steps 8 to 12: terminal showing the one-time code, then "Logged in as".
29. Part 5, step 11: GitHub device activation page.
30. Part 5, step 13: a permission request from Claude during the first save.
31. Part 5, step 14: the private repository page listing .gitignore, CLAUDE.md and the memory folder.
32. Part 5, step 15: Obsidian showing the first session log in the sessions folder.
33. Part 6, step 1: Vercel sign-up page with Continue with GitHub.
34. Part 6, step 3: the Authorize Vercel page on GitHub.
35. Part 6, step 4: Vercel plan choice screen (if shown).
36. Part 6, step 5: Vercel dashboard after sign-up.
37. Part 7, step 2: Customize > Connectors > Browse connectors directory.
38. Part 7, step 3: Notion connector card with Connect.
39. Part 7, step 4: Notion sign-in and access screen, with the workspace choice.
40. Part 7, step 5: Code tab + menu > Connectors with Notion switched on.
41. Part 7, step 6: Claude's draft summary in the Code tab.
42. Part 7, step 8: the new Notion page with the three headings.
43. If something goes wrong, item 5: /context output listing CLAUDE.md and memory/MEMORY.md under Memory files.
44. If something goes wrong, item 7: Obsidian vault name at the bottom of the left sidebar and the Manage vaults option.

---

## Sources

All checked on 5 October 2026.

**Claude**

- Plans and pricing: https://claude.com/pricing
- Sign up for the Pro plan: https://support.claude.com/en/articles/8325609-how-do-i-sign-up-for-the-pro-plan
- Download page: https://claude.com/download
- Install Claude Desktop (system requirements): https://support.claude.com/en/articles/10065433-install-claude-desktop
- Get started with the desktop app (Code tab, Local, Select folder): https://code.claude.com/docs/en/desktop-quickstart
- Desktop application reference (permission modes, terminal pane, GitHub CLI, the **+** button and Connectors in the Code tab, Customize in the sidebar): https://code.claude.com/docs/en/desktop
- Claude Code system requirements: https://code.claude.com/docs/en/setup
- How Claude remembers your project: https://code.claude.com/docs/en/memory. Facts relied on: a project CLAUDE.md is loaded at the start of every session; `@path` imports are expanded and loaded at launch alongside the CLAUDE.md that references them; relative paths resolve from the importing file; imports can nest up to four levels; text inside backticks or code blocks is skipped by the import; `/context` lists the memory files loaded in a session; auto memory is on by default in local sessions, is stored outside the project at ~/.claude/projects/<project>/memory/, and uses its own MEMORY.md index of which the first 200 lines or 25KB load at session start; the page recommends keeping each CLAUDE.md under 200 lines.
- Use connectors (Customize > Connectors > + > Browse connectors > Connect; available on Pro; connectors work in Claude Code): https://support.claude.com/en/articles/11176164-use-connectors-to-extend-claude-s-capabilities
- Notion connector listing (made by Notion; create, edit, search and organise pages): https://claude.com/connectors/notion
- Boris Cherny, creator of Claude Code, on keeping a shared CLAUDE.md and adding to it whenever Claude does something incorrectly (Threads, 2 January 2026): https://www.threads.com/@boris_cherny/post/DTBVoHZkrXC

**Obsidian**

- Download (version 1.13.7 on the date checked; Windows .exe, Mac Universal .dmg): https://obsidian.md/download
- Licence (free for all purposes including commercial use; commercial licence optional; page last updated 20 February 2025): https://obsidian.md/license
- Vaults and Open folder as vault: https://obsidian.md/help/vault (help.obsidian.md now redirects to obsidian.md/help)
- Internal links and wikilinks (links to notes in folders use the path from the vault root): https://obsidian.md/help/links
- Graph view: https://obsidian.md/help/plugins/graph
- Backlinks: https://obsidian.md/help/plugins/backlinks
- Command palette (Ctrl+P, Cmd+P): https://obsidian.md/help/plugins/command-palette
- Manage vaults (vault profile, Manage vaults): https://obsidian.md/help/manage-vaults

**Notion**

- Notion MCP (reads and writes pages; acts with your full Notion permissions): https://www.notion.com/help/notion-mcp
- Notion MCP developer overview: https://developers.notion.com/docs/mcp

**GitHub**

- Creating an account: https://docs.github.com/en/get-started/start-your-journey/creating-an-account-on-github
- Mandatory two-factor authentication: https://docs.github.com/en/authentication/securing-your-account-with-two-factor-authentication-2fa/about-mandatory-two-factor-authentication
- Configuring two-factor authentication: https://docs.github.com/en/authentication/securing-your-account-with-two-factor-authentication-2fa/configuring-two-factor-authentication
- Caching GitHub credentials in Git (GitHub CLI and Git Credential Manager): https://docs.github.com/en/get-started/git-basics/caching-your-github-credentials-in-git
- GitHub CLI: https://cli.github.com/ and https://github.com/cli/cli/releases/latest (version 2.102.0 on the date checked)
- gh auth login manual: https://cli.github.com/manual/gh_auth_login
- Git for Windows: https://git-scm.com/install/windows (version 2.56.0 on the date checked)

**Vercel**

- Hobby plan: https://vercel.com/docs/plans/hobby
- Fair use guidelines (commercial usage): https://vercel.com/docs/limits/fair-use-guidelines
- Terms of service: https://vercel.com/legal/terms
- Account management and sign-up with a Git provider: https://vercel.com/docs/accounts
- Sign-up page: https://vercel.com/signup
