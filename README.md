<!--
NOVELFLOW — GITHUB PRODUCT README
Image map (exact filenames supplied by the author):
  assets/images/1.png — Hero / brand banner
  assets/images/4.png — Library concept
  assets/images/3.png — Writing editor concept
  assets/images/2.png — Publishing concept

All four images are design concepts. They are NOT screenshots of implemented software.
Keep that distinction visible until real product screenshots replace them.
-->

<div align="center">

<img width="2172" height="724" alt="1" src="https://github.com/user-attachments/assets/181fc03c-af0e-4192-8bea-94aeacb9d851" />


# NovelFlow

### Write. Organize. Publish.

**A desktop writing and publishing studio for web novel authors.**  
One place to build your worlds, manage long-running stories, refine chapters, and prepare them for publication.

**Created by BRINKHAGEN**

![Project status](https://img.shields.io/badge/Status-In%20Development-7C5CFF?style=flat-square)
![Product stage](https://img.shields.io/badge/Stage-Concept%20%26%20Early%20Development-26324A?style=flat-square)
![Desktop](https://img.shields.io/badge/Desktop-Windows%20%7C%20macOS%20Planned-243147?style=flat-square)
![WebNovel](https://img.shields.io/badge/Publishing-WebNovel%20Inkstone%20Target-243147?style=flat-square)

**[Vision](#the-vision) · [Library](#your-stories-one-organized-library) · [Editor](#a-writing-environment-built-for-focus) · [Publishing](#publish-with-control) · [AI & EPUB](#epub-and-ai-assisted-workflows) · [Architecture](#technical-direction) · [Roadmap](#development-roadmap)**

</div>

> [!IMPORTANT]
> **NovelFlow is an independent software project in early development.** The interface images on this page are **concept previews**, not screenshots of a working release. The capabilities below describe the intended product unless explicitly stated otherwise. No stable installer or production-ready WebNovel integration is available yet.

---

## The vision

### Your story deserves more than a folder full of documents.

A serial novel may grow from ten chapters to **500, 1,000, or more**. Along the way, authors need to protect their manuscript, keep a consistent story world, find the right chapter, and prepare new releases without losing hours to repetitive publishing tasks.

Most of that work happens across separate applications. NovelFlow is being designed to connect it into one coherent experience:

| **WRITE** | **ORGANIZE** | **PUBLISH** |
| :-- | :-- | :-- |
| Shape scenes and chapters in a focused editor. | Keep books, volumes, drafts, notes, and story details together. | Prepare, review, and transfer approved chapters to supported platforms. |
| Rich text and distraction-free tools. | Structure that scales with long-running series. | A publishing queue with clear status and verification. |

**One manuscript. One organized workspace. A deliberate publishing workflow.**

### From a manuscript to a release

```mermaid
flowchart LR
    A["Import or start a manuscript"] --> B["Organize chapters"]
    B --> C["Write and revise"]
    C --> D["Review and approve"]
    D --> E["Publishing queue"]
    E --> F["Platform transfer"]
    F --> G["Verify publication status"]
```

*This diagram describes the intended workflow, not an implemented end-to-end pipeline.*

---

## Designed for stories that keep growing

NovelFlow is envisioned as a local-first application built around the way serial fiction is actually written and released.

| Product area | Intended experience | Stage |
| :-- | :-- | :-- |
| **Novel library** | Multiple novels, books, volumes, chapters and drafts | Planned |
| **Rich-text editor** | Focused writing, formatting, word count and autosave | Planned |
| **Editorial workflow** | Draft → Review → Ready → Queued → Published | Planned |
| **EPUB import** | Extract and organize chapters from authorized manuscripts | Planned |
| **Publishing integration** | Browser-assisted chapter transfer to Inkstone | Research / planned |
| **Release planning** | Queue management and verified scheduling where supported | Research / planned |
| **Series Bible** | Characters, locations, lore, terminology and continuity | Future |
| **AI workspace** | Optional editing, translation and narrative assistance | Future |
| **Additional platforms** | Independent adapters for other serial-fiction sites | Future |

**Local-first** means the author should remain in control of the original manuscript. A publishing website is a destination, not the only place where a story exists.

---

## Your stories. One organized library.

<img src="assets/images/4.png" alt="NovelFlow Library — proposed desktop interface with novel cards, chapters and progress overview" width="100%">

<p align="center"><sub>DESIGN CONCEPT 01 — LIBRARY · Illustrative interface, not an application screenshot.</sub></p>

### See the entire writing universe at a glance

A scalable library is central to NovelFlow's design. It should help authors manage multiple series without digging through hundreds of independent files.

**Planned library capabilities**

- **Books and series:** Organize related projects inside one workspace.
- **Volumes and chapters:** Navigate thousands of numbered chapters in a clear hierarchy.
- **Draft inbox:** Keep new or unsorted work separate from approved manuscripts.
- **Project overview:** See writing progress, status, word counts, and recently edited chapters.
- **Search and filtering:** Find chapters, notes, titles, and tagged content.
- **Metadata:** Track chapter order, language, revision state and local publishing history.

```text
My Library
└── The Shattered Realms
    ├── Volume 01 — Awakening
    │   ├── Chapter 001 — Prologue          [Published]
    │   ├── Chapter 002 — A Fractured Sky  [Published]
    │   ├── Chapter 003 — Echoes           [Published]
    │   └── Chapter 023 — First Contact    [Draft]
    ├── Volume 02 — The Lost Empire
    └── Unsorted Drafts
```

The title and chapter information above are examples of the proposed data structure.

---

## A writing environment built for focus

<img src="assets/images/3.png" alt="NovelFlow Editor — concept interface with chapter navigation, rich-text manuscript and contextual notes" width="100%">

<p align="center"><sub>DESIGN CONCEPT 02 — WRITING EDITOR · Proposed layout and tools.</sub></p>

### Every chapter in its place. Every word under your control.

NovelFlow's editor is designed for writers who want a full manuscript workspace without the complexity of a general-purpose office suite.

| Editing tools | Manuscript intelligence | Workspace comfort |
| :-- | :-- | :-- |
| Bold, italic, headings, lists, quotes | Word and character counts | Focused, distraction-reduced layout |
| Undo/redo and keyboard shortcuts | Chapter and volume navigation | Contextual notes panel |
| Search and replace | Draft and revision status | Autosave and local recovery |
| Structured document model | Revision history (later milestone) | Adjustable display preferences |

### A safer approach to manuscript editing

The **source manuscript** should never be overwritten just because the author prepares a version for a publishing platform.

```text
Original Manuscript
       │
       ├── Working Draft
       │      └── Editorial Review
       │                └── Approved Chapter
       │
       └── Local Backup / Export
                              │
                              └── Platform-Specific Publishing Copy
```

This separation is a **design requirement**, not a claim that backup or version control is already implemented.

---

## Publish with control

<img src="assets/images/2.png" alt="NovelFlow Publishing — concept interface for chapter queue, release controls and browser-assisted transfer" width="100%">

<p align="center"><sub>DESIGN CONCEPT 03 — PUBLISHING CENTER · Planned integration and controls.</sub></p>

### Prepare fifty chapters. Review them individually. Release deliberately.

NovelFlow's first intended publishing destination is **WebNovel Inkstone**. Its publishing module is planned around a reviewable queue, not an uncontrolled one-click mass-publication promise.

**Proposed publishing sequence**

1. Select chapters marked **Ready** in the NovelFlow manuscript.
2. Validate chapter order, title, length and required fields.
3. Prepare a platform-compatible copy without changing the source document.
4. Open the platform in an authenticated browser session controlled by the author.
5. Transfer chapter content and request a draft or publication action where supported.
6. Verify the result before marking the local chapter as uploaded or published.
7. Record errors and keep unfinished work in the queue for retry or manual review.

### A publishing queue authors can trust

| Local state | Meaning |
| :-- | :-- |
| **Draft** | Still being written or edited |
| **In review** | Awaiting author approval |
| **Ready** | Approved for transfer |
| **Queued** | Awaiting the chosen publishing action |
| **Uploaded** | Transfer reported successful; remote state still needs validation |
| **Scheduled** | Future publication confirmed by the target platform, where supported |
| **Published** | Publication verified on the target platform |
| **Needs attention** | Validation, transfer or verification failed |

The separation between **Uploaded**, **Scheduled**, and **Published** is intentional: an upload is not automatically proof that a chapter is publicly visible.

### About WebNovel / Inkstone compatibility

There is no officially supported public chapter-upload API on which this project currently relies. The initial integration concept uses a **browser-based adapter** operating through the site's regular interface.

- Authors should authenticate on the platform's own login page.
- NovelFlow should not ask for or store the WebNovel account password.
- Untrusted remote pages must remain isolated from privileged desktop capabilities.
- Transfers need validation, duplicate prevention, error recovery and an audit trail.
- Platform changes, anti-automation controls and terms may limit or interrupt automation.
- **Batch importing hundreds of chapters and scheduling releases remain unverified development goals.**

NovelFlow is not an official WebNovel client. Features will only be marked as supported after real integration testing.

---

## EPUB and AI-assisted workflows

### From source material to a carefully reviewed manuscript

One major product direction is a workspace that can import **EPUB manuscripts**, detect chapters and help develop new writing projects with structured editorial assistance.

```text
Authorized EPUB / manuscript
           ↓
  Import and chapter parsing
           ↓
 Source library + metadata
           ↓
 Story structure / terminology
           ↓
 Write · Translate · Edit · Compare
           ↓
      Human review
           ↓
     Approved chapters
           ↓
       Publish queue
```

**Planned import capabilities** include EPUB, Markdown, TXT and HTML. DOCX and additional formats are possible future extensions. The eventual export pipeline is intended to provide portable manuscripts rather than lock the author into one editor.

### Optional AI workspace — future direction

AI assistance should work with **relevant story context**, not treat chapter 300 as an isolated prompt with no memory of earlier chapters.

Potential tools include:

- **Chapter drafting and revision:** Improve flow, clarity, dialogue and narrative pacing.
- **Series Bible integration:** Consult character profiles, locations, rules of the fictional world and established facts.
- **Continuity checks:** Flag contradictory character details, plot events and timeline conflicts for review.
- **Translation and localization:** Compare source, draft translation and approved target-language text.
- **Terminology control:** Keep proper names, invented terms, titles and repeated concepts consistent.
- **Side-by-side review:** Preserve the source while evaluating AI-assisted revisions.
- **Provider choice:** Connect supported AI services without making AI mandatory for ordinary writing.

> [!NOTE]
> **AI features are a future module, not a current product capability.** Third-party AI services may have separate usage charges and terms. Importing or transforming a book does **not** grant copyright or publishing rights. Authors must own or have appropriate permission to adapt, translate and publish the source material.

---

## A modular publishing foundation

A strong manuscript editor should not have to change every time a publishing website changes.

NovelFlow is designed around independent publishing adapters, each responsible for its own platform-specific transfer, verification and error-handling logic.

```text
                     NOVELFLOW DESKTOP
┌──────────────────────────────────────────────────┐
│                    Workspaces                    │
│    Library  ·  Editor  ·  Notes  ·  Publishing    │
├──────────────────────────────────────────────────┤
│            Structured Manuscript Core            │
│         Books  ·  Volumes  ·  Chapters            │
├──────────────────────────────────────────────────┤
│  Import / Export  │  Local Storage  │  Backups    │
├──────────────────────────────────────────────────┤
│             Publishing Adapter Layer             │
│       WebNovel first  ·  Others later            │
├──────────────────────────────────────────────────┤
│         Optional AI / Translation Workspace      │
└──────────────────────────────────────────────────┘
```

### Intended platform roadmap

| Destination | Direction | Status |
| :-- | :-- | :-- |
| **WebNovel / Inkstone** | First experimental publishing adapter | Planned |
| **Royal Road** | Possible future publishing adapter | Future |
| **Scribble Hub** | Possible future publishing adapter | Future |
| **Other platforms** | Added selectively, subject to technical feasibility and site rules | Exploratory |

Individual adapters should expose clear capabilities rather than promise identical features on every website. A platform that does not support scheduling, for example, should not appear to offer verified native scheduling inside NovelFlow.

---

## Technical direction

NovelFlow's proposed first-generation stack focuses on a polished cross-platform desktop interface and local manuscript ownership.

| Layer | Proposed technology / principle |
| :-- | :-- |
| **Desktop runtime** | Electron |
| **User interface** | React + TypeScript |
| **Manuscript editor** | Structured rich-text editing model; implementation to be selected |
| **Local project store** | SQLite |
| **Imports and exports** | EPUB / Markdown / TXT / HTML processing modules |
| **Publishing** | Per-platform adapters with carefully isolated browser sessions |
| **Localization** | Interface and content languages treated separately |
| **AI** | Optional provider integrations in a later phase |

### Local-first, secure by design

**Security requirements for implementation**

- Strong Electron isolation: sandboxed remote content, context isolation, minimal preload APIs and no privileged Node.js access in untrusted pages.
- Narrow, validated IPC boundaries between the desktop shell and application features.
- Sensitive account or token data excluded from logs, repositories and manuscript exports.
- Local backups and recovery designed into the manuscript storage lifecycle.
- Import size limits, file validation and safe handling of untrusted documents.
- Clear confirmation and result verification for publishing actions.
- Separation between a user's local manuscript data and third-party platform sessions.

These are **engineering requirements**; an actual security audit can only happen once the application and integrations exist.

### Language-aware publishing

NovelFlow aims to distinguish between:

| Setting | Example |
| :-- | :-- |
| Interface language | German |
| Manuscript language | English |
| Source language | Chinese |
| Target translation language | English |
| Publishing language | English |

Initial interface localization is planned for English and German. Further languages can be added through the localization system as the product develops.

---

## Development roadmap

This roadmap describes scope, **not completed functionality**. Boxes will be checked only after implementation and testing.

<details open>
<summary><strong>Phase 01 — Desktop & manuscript foundation</strong></summary>

- [ ] Electron shell, navigation and application settings
- [ ] Project creation and local database
- [ ] Books, volumes, chapters and ordering
- [ ] Rich-text editing and chapter metadata
- [ ] Autosave, document recovery and local backups
- [ ] Search, word counts, chapter status and keyboard shortcuts

</details>

<details>
<summary><strong>Phase 02 — Import, editorial workflow & portability</strong></summary>

- [ ] EPUB, Markdown, TXT and HTML ingestion
- [ ] Safe chapter extraction and import preview
- [ ] Import conflict detection and ordering tools
- [ ] Revision and approval workflow
- [ ] Platform-independent manuscript export
- [ ] Restoration tests and data migration strategy

</details>

<details>
<summary><strong>Phase 03 — WebNovel publishing prototype</strong></summary>

- [ ] Browser session integration and authentication boundaries
- [ ] Target-site editor detection and compatibility tests
- [ ] Chapter title and content transfer
- [ ] Draft save and manual review where supported
- [ ] Upload verification, duplicate checks and recoverable errors
- [ ] Publishing queue, logs and remote status reconciliation
- [ ] Scheduling feasibility assessment with small test batches

</details>

<details>
<summary><strong>Phase 04 — Professional author tools</strong></summary>

- [ ] Series Bible and character relationship tracking
- [ ] Worldbuilding, glossary and timeline
- [ ] Revision history and comparison tools
- [ ] Writing goals, progress insights and project templates
- [ ] Multi-language user interface
- [ ] Additional publishing adapters

</details>

<details>
<summary><strong>Phase 05 — Optional AI studio</strong></summary>

- [ ] Configurable AI provider connections
- [ ] Rights-aware source-manuscript workflows
- [ ] Story context retrieval across chapters
- [ ] Chapter editing and drafting assistance
- [ ] Translation review and terminology checks
- [ ] Character and plot continuity analysis
- [ ] Privacy and cost controls for AI usage

</details>

---

## Product principles

| Principle | Why it matters |
| :-- | :-- |
| **The author's manuscript comes first** | No third-party publishing service should become the only copy of a story. |
| **Human approval matters** | AI editing and automated publishing must remain reviewable. |
| **No false publishing success** | Remote publication status must be verified. |
| **Modular integrations** | Changes to one website should not break the entire writing environment. |
| **Transparent capabilities** | A concept, prototype and production-ready feature are not the same thing. |
| **Portable work** | Authors should be able to export and preserve their manuscripts. |

---

## Current status

> **Concept & early development.** At this stage, NovelFlow is a documented product vision, not a generally available writing application. The four images on this page visualize design direction and proposed behavior. They do not demonstrate completed functionality.

**Not available yet:** a public installer, a stable release, an authenticated WebNovel integration, a verified 500-chapter import, and automated scheduling.

Development priorities may change as the core editor, data model and publishing feasibility are tested.

## Questions & answers

<details>
<summary><strong>Is NovelFlow available for download?</strong></summary>

Not yet. This repository currently presents the product direction and development plan. A release will be announced only when a real, tested build exists.

</details>

<details>
<summary><strong>Does NovelFlow work without an internet connection?</strong></summary>

Offline manuscript editing is a core design goal. Publishing to third-party platforms and using cloud AI services will require an internet connection.

</details>

<details>
<summary><strong>Can NovelFlow publish 500 chapters automatically?</strong></summary>

Not currently. Managing very large manuscripts and reducing repetitive publishing work are primary goals, but bulk transfer, draft handling and scheduling must be tested against the actual platform. Availability will depend on technical compatibility and platform rules.

</details>

<details>
<summary><strong>Will it rewrite any EPUB into a publishable novel?</strong></summary>

EPUB import and AI-assisted editorial work are planned. Publishing an adaptation or translation requires the necessary rights; changing wording with AI does not automatically make third-party material free to publish.

</details>

<details>
<summary><strong>Is this affiliated with WebNovel or Inkstone?</strong></summary>

No. NovelFlow is an independent BRINKHAGEN project. Third-party platform names identify potential integration targets only.

</details>

---

## Brand, independence & rights

**NovelFlow** is designed and developed by **BRINKHAGEN** as an independent software project.

This project is **not affiliated with, endorsed by, sponsored by or officially connected to** WebNovel, Inkstone, Royal Road, Scribble Hub or their respective owners. All third-party names, logos and trademarks remain the property of their respective owners.

**Repository license:** No open-source software license has been published for this project at this stage. Unless a license is explicitly added, all rights are reserved. The design concepts on this page are illustrative and are not an invitation to redistribute the artwork.

---

<div align="center">

### NovelFlow

**Write. Organize. Publish.**

*Your next chapter starts here.*

**Developed by BRINKHAGEN**  
© 2026 BRINKHAGEN. All rights reserved.

</div>
