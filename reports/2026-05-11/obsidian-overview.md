---
title: "Obsidian: A One-Page Overview"
date: "2026-05-11"
author: "Patrick"
---

# Obsidian: A One-Page Overview

## What it is

Obsidian is a desktop and mobile note-taking app that stores notes as plain markdown files in a local folder it calls a "vault." There is no proprietary database — your notes remain readable in any text editor, today and ten years from now. The app layers a fast editor, a rich linking system, and an extensible plugin runtime on top of that flat folder.

## Key features

### Local-first markdown

Every note is a `.md` file on disk. You own the files, back them up however you want, and edit them with any tool. No vendor lock-in.

### Linking and backlinks

Wiki-style `[[double-bracket]]` links connect notes. Every note shows incoming references (backlinks) automatically, turning a folder of files into a personal knowledge graph without manual upkeep. Unlinked-mention search surfaces implicit connections.

### Graph view

A force-directed visualization of all notes and their links. Useful for spotting clusters, orphan notes, and the overall shape of your knowledge base. Local graphs scope the view to one note's neighborhood.

### Plugins

Two flavors: core plugins (shipped, toggle on/off) and community plugins (1,500+ third-party). Common picks include Dataview (query notes as a database), Templater (scripted templates), Tasks (GTD-style task tracking), and Excalidraw (hand-drawn diagrams inside notes). The plugin API is generous enough that Obsidian functions as a small platform, not just an app.

### Sync options

- **Obsidian Sync** — paid first-party service ($4/mo), end-to-end encrypted, handles conflict resolution.
- **iCloud / Dropbox / Google Drive** — free, works for single-device-at-a-time use, fragile under concurrent edits.
- **Git** — popular with developers; full history, free, requires comfort with merge conflicts.
- **Self-hosted (Syncthing, rclone)** — free, peer-to-peer, no cloud middleman.

## Who it's for

Knowledge workers, researchers, students, and developers who want durable plain-text notes and are willing to assemble their own workflow. Obsidian rewards customization; it punishes users who want a turnkey, opinionated experience out of the box.

## How it compares

| Dimension | Obsidian | Notion | Logseq |
|-----------|----------|--------|--------|
| Storage | Local markdown files | Cloud-only (proprietary blocks) | Local markdown or org-mode |
| Offline | First-class | Limited | First-class |
| Collaboration | Weak (single-user focus) | Strong (real-time multi-user) | Weak |
| Structure | Pages + links | Databases + pages | Outliner (bullet-first) |
| Extensibility | Large plugin ecosystem | Limited (API + integrations) | Smaller plugin ecosystem |
| Price | Free personal; $50/yr commercial | Free tier; paid teams | Free, open source |
| Best for | Personal knowledge graphs | Team wikis and project hubs | Daily-journal-driven thinking |

**Short version:** pick Obsidian if you want local files and a thriving plugin scene; Notion if you need real-time collaboration and structured databases; Logseq if you think in outlines and want fully open-source tooling.

## Bottom line

Obsidian is the strongest single-user, local-first markdown knowledge tool available in 2026. Its plain-text foundation makes it future-proof, and the plugin ecosystem covers nearly any workflow you can describe. The tradeoff is upfront configuration — you build your system rather than receive one.
