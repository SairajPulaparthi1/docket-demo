# Docket

**A personal, local-first ticket board. Jira's structure, a to-do app's simplicity, and your files stay on your machine.**

**[Try the live demo →](https://sairajpulaparthi1.github.io/docket-demo/)** (saved only in your browser)

The demo board is a real example: how I track my other project, **[Brightside PM Sim](https://sairajpulaparthi1.github.io/brightside-pm-sim/)**, a game that teaches product management. Shipped weeks are in Done, Week 4 is in progress, and there's a bug, a playtest plan, ideas, and reference notes like "how to push an update".

## The idea

Most to-do apps are too thin for real work, and team tools like Jira are too heavy for one person. Docket sits in between:

- **A Today page.** A greeting, how much you finished this week, and three lists: what needs your call, what is in progress, and what is up next. Tick the box to finish a ticket.
- **A real board.** Backlog → To Do → In Progress → Waiting for Review → Blocked → Done, with projects, priorities, labels and due dates. Drag cards between columns.
- **Tickets that hold the whole story.** Markdown descriptions, checklists, links, timestamped notes, an activity log, and attached files (drag-drop or paste a screenshot).
- **Search that reads your files.** ⌘K searches titles, notes, labels *and the text inside attached logs, Markdown, code, PDFs and Word documents*.
- **A library, not just a board.** Notes, references and ideas (commands, how-tos, snippets) live next to your tickets.
- **Local-first.** Every ticket is a plain JSON file and every attachment a normal file on disk. Nothing is uploaded; you can grep it, back it up or edit it by hand.
- **Works from the terminal.** A `docket` command (`docket add`, `docket note`, `docket done`, `docket search`, …) reads and writes the same files, and the app picks up changes within seconds.
- **Hands work to an AI coding agent.** "Send to Claude" opens a Claude Code session in the project's folder, already briefed with the ticket, and the agent logs its progress back to the ticket as it works.

## About this demo

The desktop app is a tiny local Node server plus a single-page UI. This demo is that same UI running entirely in your browser, with the server swapped for an in-page stand-in and seeded with that example board. Your changes are kept in your browser's storage; **Reset** (bottom left) restores the sample data.

Not available in the demo: opening files in Finder, backups to disk, and actually launching Claude Code (you can still preview and copy the brief).

Keyboard: `C` create · `⌘K` or `/` search · `1`–`5` switch views (Today, Board, List, Library, Files) · `Esc` close.
