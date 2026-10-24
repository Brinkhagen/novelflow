<!--
NOVELFLOW — README IMAGE GUIDE

To add an image later, upload it to the stated repository path and replace the
matching IMAGE SLOT comment with the Markdown line printed inside that comment.
Until then, these comments are invisible on GitHub and no broken image appears.

01  HERO:       assets/branding/novelflow-hero.png             (1600 × 500 px)
02  LIBRARY:    assets/screenshots/library-preview.png        (1440 × 900 px)
03  EDITOR:     assets/screenshots/editor-preview.png         (1440 × 900 px)
04  PUBLISHING: assets/screenshots/publishing-preview.png     (1440 × 900 px)

Use "Concept Preview" on mockups until actual application screenshots exist.
-->

<!-- IMAGE SLOT 01 — HERO BANNER
Upload: assets/branding/novelflow-hero.png
Replace this whole comment with:
![NovelFlow — Write. Organize. Publish.](assets/branding/novelflow-hero.png)
-->

<h1 align="center">NovelFlow</h1>

<p align="center"><strong>Write. Organize. Publish.</strong></p>

<p align="center">A modern desktop writing and publishing studio for serialized fiction and web novel authors.</p>

<p align="center"><em>Designed for long-running stories. Built by BRINKHAGEN.</em></p>

<p align="center"><strong>Status:</strong> Early development · <strong>Platforms:</strong> Windows / macOS (planned) · <strong>First publishing target:</strong> WebNovel Inkstone</p>

---

## The idea

Writing a 500-chapter novel should not mean managing hundreds of disconnected documents, losing track of characters, or copying each chapter into a publishing website by hand.

**NovelFlow** aims to bring the entire workflow into one focused desktop application:

**Import → Organize → Write & Revise → Review → Queue → Publish**

The project is currently in **early development**. The interfaces and capabilities described below are product goals, **not claims that a complete app is already available**.

## A workspace built for long-form fiction

| Writing | Organization | Publishing |
| --- | --- | --- |
| Rich-text chapter editor | Books, volumes and chapters | WebNovel / Inkstone integration (planned) |
| Autosave and revision history | Drafts, notes and chapter status | Draft transfer and review (planned) |
| Word and character counts | Large-series navigation | Publishing queue (planned) |
| Search and replace | Series Bible and continuity tools (future) | Additional platform adapters (future) |

### Your library, at a glance

<!-- IMAGE SLOT 02 — LIBRARY PREVIEW
Upload: assets/screenshots/library-preview.png
Replace this whole comment with:
![NovelFlow library — concept preview](assets/screenshots/library-preview.png)
-->

**Planned:** Keep multiple books in a structured library, with volumes, numbered chapters, unsorted drafts, search, and clear progress indicators.

```text
My Library
└── Book: The First Ascendant
    ├── Volume 01 — Awakening
    │   ├── Chapter 001 — Exile           [Draft]
    │   ├── Chapter 002 — The Signal      [Ready]
    │   └── Chapter 003 — First Contact   [Ready]
    ├── Volume 02 — New Horizons
    └── Unsorted Drafts
```

### A writing space that stays out of the way

<!-- IMAGE SLOT 03 — EDITOR PREVIEW
Upload: assets/screenshots/editor-preview.png
Replace this whole comment with:
![NovelFlow rich-text editor — concept preview](assets/screenshots/editor-preview.png)
-->

**Planned editor capabilities:**

- Rich-text formatting: bold, italic, headings, lists, quotes and alignment
- Distraction-free writing, keyboard shortcuts and focus mode
- Automatic saving, local drafts and revision history
- Word count, character count, search and replace
- Structured document storage to preserve the manuscript independently of any publishing platform

## From manuscript to publication

<!-- IMAGE SLOT 04 — PUBLISHING PREVIEW
Upload: assets/screenshots/publishing-preview.png
Replace this whole comment with:
![NovelFlow publishing queue — concept preview](assets/screenshots/publishing-preview.png)
-->

NovelFlow's first publishing integration is intended for **WebNovel Inkstone**. Because no officially supported public chapter-upload API is currently assumed, the planned approach uses a browser-based publishing adapter.

```text
NovelFlow manuscript
        ↓
Select and validate chapters
        ↓
Publishing queue
        ↓
WebNovel Inkstone in an embedded browser
        ↓
Transfer title and formatted content
        ↓
Save as draft → Review → Publish
        ↓
Record the result locally
```

The goal is to let authors prepare many chapters, review transfers, and publish without repeated copy-and-paste.

**Publishing safeguards (planned):**

- User signs in on WebNovel's own website, not in a NovelFlow password form
- Explicit confirmation before publishing chapters
- Detection of failed or duplicate transfers
- Local status tracking for pending, uploaded and published chapters
- Platform-specific formatting conversion that does not overwrite the original manuscript
- Scheduling support **only where technically available and verified**

Browser automation can break when a publishing platform changes its interface, and platform rules still apply. **A 500-chapter batch upload or scheduled release is a target to test, not a currently verified feature.**

## EPUB import, translation and AI-assisted workflows

A major long-term goal is a source-to-manuscript workspace for large stories.

**Planned workflow:**

1. Import an EPUB, TXT, HTML or Markdown manuscript.
2. Detect the book structure and extract chapters.
3. Organize chapters, characters, terminology and story context.
4. Translate, rewrite or develop authorized material with optional AI assistance.
5. Compare source and edited drafts side by side.
6. Review the final text and move approved chapters to the publishing queue.

Potential AI tools include chapter editing, grammar and dialogue improvements, style checks, Series Bible references, timeline checks, character consistency and continuity detection.

**AI is optional and is not built into the initial release.** Future integrations may use third-party API keys, with separate provider costs. Authors are responsible for having the rights needed to adapt, translate or publish imported content.

## Architecture (proposed)

NovelFlow is planned as a local-first cross-platform desktop application.

```text
NovelFlow Desktop
├── Electron
│   ├── React + TypeScript interface
│   └── Secure embedded browser for publishing
├── Writing & Organization
│   ├── Rich-text document model
│   ├── Books / volumes / chapters
│   └── Search, drafts and revision history
├── Local Storage
│   ├── SQLite project data
│   └── Backups and manuscript exports
├── Import / Export
│   ├── EPUB, Markdown, TXT and HTML (planned)
│   └── DOCX and additional formats (future)
├── Publishing Adapters
│   ├── WebNovel / Inkstone (first target)
│   └── Other platforms (future)
└── Optional AI Workspace (future)
    ├── Model-provider connections
    ├── Series Bible / context
    └── Translation and editing tools
```

### Local-first by design

Manuscripts should remain usable without a publishing account or an always-on internet connection. Online access is needed for platform publishing and any connected cloud AI services.

**Security priorities:** context isolation, narrow IPC permissions, no direct Node.js access for untrusted website content, validated imports, encrypted sensitive local data where appropriate, and no publishing credentials committed to Git.

## Roadmap

The roadmap represents planned work. Items will be checked off **only after they have been implemented and tested**.

### Phase 1 — Writing foundation

- [ ] Electron desktop application and navigation
- [ ] Local project database and backup strategy
- [ ] Book, volume and chapter management
- [ ] Rich-text editor, autosave and search
- [ ] Chapter status and writing statistics

### Phase 2 — Import and editorial workflow

- [ ] EPUB, Markdown, TXT and HTML import
- [ ] Chapter extraction and ordering
- [ ] Side-by-side manuscript review
- [ ] Import validation and export tools

### Phase 3 — WebNovel publishing

- [ ] Secure embedded browser and Inkstone login
- [ ] Chapter title and content transfer
- [ ] Draft upload, verification and error handling
- [ ] Publishing queue and status tracking
- [ ] Scheduling research and controlled testing

### Phase 4 — Professional and AI workflows

- [ ] Series Bible, characters and worldbuilding
- [ ] Timeline and continuity tools
- [ ] Optional AI provider integration
- [ ] Translation and localization workflows
- [ ] Additional publishing platform adapters

## Development status & availability

> **Early development / not production-ready.** The repository currently documents the product direction. No stable NovelFlow installer or finished publishing integration is being offered here yet.

Screenshots added during this stage will be labeled **Concept Preview** until they show real implemented features.

## Independence & trademarks

NovelFlow is an independent project developed by **BRINKHAGEN**. It is not affiliated with, endorsed by, sponsored by or officially connected to WebNovel, Inkstone, Royal Road, Scribble Hub or their respective owners. Third-party names and trademarks belong to their owners.

## License

No open-source license has been declared for this repository at this stage. Unless a separate license is added, all rights are reserved.

---

<h3 align="center">NovelFlow</h3>

<p align="center"><strong>Write. Organize. Publish.</strong></p>

<p align="center"><em>Developed by BRINKHAGEN</em></p>

<p align="center">© 2026 BRINKHAGEN. All rights reserved.</p>
