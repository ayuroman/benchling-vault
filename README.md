# benchling-vault
Transform raw Benchling exports into an interconnected and fully offline Markdown vault.

> **Disclaimer:** This project is an independent open-source tool and is not affiliated with, endorsed by, or sponsored by Benchling.


## The Problem

* **Platform Lock-in:** Cloud ELNs leave experimental history vulnerable to SSO deactivation, institutional license expiration, and unexpected network outages.
* **Siloed Data:** Once downloaded, raw exports break internal hyperlinks between protocols, notebook entries, and registry items.
* **Dead Backups:** Raw Benchling exports dump unwieldy, deeply nested folder structures with 200+ character filenames that frequently fail to sync on OneDrive or SharePoint due to `MAX_PATH` limits.


## The Solution

* **Zero-Cloud Processing:** 100% client-side execution - unpublished data never touches an external server.
* **Interconnected Graph:** Converts Benchling internal links into standard wikilinks (`[[Note Name]]`) ready for Obsidian and Logseq.
* **Clean File Hierarchy:** Flattens and sanitizes unwieldy export paths into a clean, desktop-friendly directory structure.
* **Local AI Ready:** Generates plain-text Markdown formatted for local RAG and offline LLM indexing (e.g., Ollama, Smart Connections) without risking IP leaks.
