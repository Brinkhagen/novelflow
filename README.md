<div align="center">

# NovelFlow

### Write. Organize. Publish.

**A professional desktop writing and publishing studio for web novel authors.**

Built by **Brinkhagen**.

<br>

![Status](https://img.shields.io/badge/status-in%20development-c9a96e)
![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20macOS-blue)
![Desktop](https://img.shields.io/badge/desktop-Electron-47848F)
![Language](https://img.shields.io/badge/UI-multilingual-success)

</div>

---

## About NovelFlow

NovelFlow is a modern desktop workspace designed for authors who publish serialized fiction and web novels.

It combines a distraction-free writing environment, structured book and chapter management, rich-text editing, and publishing tools in one application.

Instead of writing in one application, organizing chapters somewhere else, and manually copying every chapter into a publishing platform, NovelFlow brings the complete workflow into a single workspace.

> Write your story. Organize your chapters. Publish when you're ready.

---

## Core Features

### Professional Writing Editor

Write directly inside NovelFlow using a modern rich-text editor designed for long-form fiction.

Planned editor features include:

- Bold
- Italic
- Underline
- Headings
- Section breaks
- Lists
- Blockquotes
- Text alignment
- Undo / Redo
- Find and Replace
- Word count
- Character count
- Focus mode
- Keyboard shortcuts
- Automatic saving
- Revision history

NovelFlow stores manuscripts in a structured document format so content can later be exported cleanly to different formats and publishing platforms.

---

## Books, Volumes & Chapters

NovelFlow is designed to keep even very large serialized novels organized.

```text
Book
├── Volume 1
│   ├── Chapter 001
│   ├── Chapter 002
│   └── Chapter 003
│
├── Volume 2
│   ├── Chapter 004
│   └── Chapter 005
│
└── Unsorted Drafts

Each chapter can contain its own:
- Title
- Word count
- Notes
- Status
- Last edited date
- Publishing status
- Platform metadata
Chapter Workflow
NovelFlow uses a simple publishing workflow:
Draft
   ↓
Ready
   ↓
Uploaded
   ↓
Published

This makes it easy to see which chapters are still being written, which are ready for review, and which have already been published.
Inkstone / WebNovel Publishing
One of NovelFlow's first publishing integrations is planned for WebNovel Inkstone.
Users authenticate directly with WebNovel through an embedded browser session.
NovelFlow does not need to store the user's WebNovel password.
The publishing workflow is designed around:
- Opening Inkstone inside NovelFlow
- Logging into WebNovel directly
- Selecting ready chapters
- Automatically filling chapter titles
- Transferring chapter content
- Preserving supported formatting
- Saving chapters as drafts
- Reviewing chapters before publication
- Publishing selected chapters
- Tracking local and remote publishing status
Example workflow:
NovelFlow Editor
       ↓
Ready for Publishing
       ↓
Inkstone
       ↓
Upload as Draft
       ↓
Review
       ↓
Publish

Publishing automation is intended to keep authors in control of every release.
Publishing Queue
Authors can prepare multiple chapters before uploading them.
Example:
Chapter	Words	Status
Chapter 021 — The Arrival	2,840	Published
Chapter 022 — The Fleet	3,120	Published
Chapter 023 — The Golden Fleet	2,481	Ready
Chapter 024 — First Contact	3,054	Ready
Chapter 025 — A New Threat	2,910	Draft


Ready chapters can then be processed through the publishing workspace.
Integrated Browser
NovelFlow is being designed as a desktop application with an embedded Chromium environment.
This allows supported publishing platforms to run directly inside NovelFlow while keeping authentication inside the platform's own website.
┌──────────────────────── NovelFlow ────────────────────────┐
│                                                          │
│ Chapters       Writing Editor          Publishing         │
│                                                          │
│ Chapter 23     Your manuscript...      WebNovel ✓         │
│ Chapter 24                              Royal Road         │
│ Chapter 25                              Future Platforms   │
│                                                          │
└──────────────────────────────────────────────────────────┘

The embedded browser is planned to support:
- Persistent local login sessions
- Inkstone navigation
- Chapter editor detection
- Chapter title transfer
- Chapter content transfer
- Draft creation
- Manual review before publishing
- Publishing queue processing
Rich-Text Formatting
NovelFlow is not intended to be a plain-text editor.
The editor is planned to support structured rich-text content including:
- Bold
- Italic
- Underline
- Headings
- Paragraphs
- Lists
- Quotes
- Horizontal separators
- Alignment
- Links
- Supported inline formatting
The editor will use a structured internal document model so formatting can be converted per publishing platform.
Example:
NovelFlow Rich Text
        ↓
Platform Adapter
        ↓
Inkstone-Compatible Content

Unsupported formatting can be simplified safely during publishing without changing the manuscript stored inside NovelFlow.
Multilingual by Design
NovelFlow is designed from the beginning for international authors.
The application architecture separates:
- Interface language
- Book language
- Source language
- Target language
- Publishing language
Example:
Interface Language: German
Book Language: English
Source Language: Chinese
Target Language: English
Publishing Language: English

Initial interface languages are planned to include:
- English
- German
Additional languages can be added through the localization system.
Import & Export
Planned Import Formats
- Markdown
- TXT
- HTML
Planned Export Formats
- Markdown
- TXT
- HTML
- DOCX
- EPUB
Additional formats may be added later.
Platform Integrations
NovelFlow is designed around a modular publishing adapter architecture.
Planned
- WebNovel / Inkstone
Future
- Royal Road
- Scribble Hub
- Additional serialized-fiction platforms
Each publishing integration is separated from the core writing environment.
This allows platform-specific changes to be updated without affecting the entire application.
Desktop Architecture
NovelFlow is planned as a modern cross-platform desktop application.
Core technologies:
Desktop
└── Electron

Interface
├── React
└── TypeScript

Editor
└── Structured Rich Text

Local Application Data
└── SQLite

Publishing
└── Chromium-based platform adapters

Localization
└── i18n

This architecture allows NovelFlow to function locally while leaving room for future cloud synchronization and account-based services.
Privacy & Authentication
NovelFlow is designed so third-party publishing credentials do not need to be stored by NovelFlow.
Where possible, authentication takes place directly inside the publishing platform's own browser environment.
Example:
User
 ↓
Embedded Chromium
 ↓
WebNovel Login
 ↓
Authenticated Local Browser Session

NovelFlow should never require users to provide their publishing password directly to NovelFlow.
Sensitive authentication information must never be committed to this repository.
Product Roadmap
Phase 1 — Writer
- [ ] Desktop application shell
- [ ] User interface
- [ ] Project creation
- [ ] Book management
- [ ] Volume management
- [ ] Chapter management
- [ ] Rich-text editor
- [ ] Autosave
- [ ] Word counting
- [ ] Character counting
- [ ] Chapter status workflow
- [ ] Search
- [ ] Find and Replace
- [ ] Keyboard shortcuts
Phase 2 — Publishing
- [ ] Embedded Chromium browser
- [ ] WebNovel authentication session
- [ ] Inkstone detection
- [ ] Chapter title transfer
- [ ] Chapter content transfer
- [ ] Formatting conversion
- [ ] Draft upload
- [ ] Manual review workflow
- [ ] Publishing queue
- [ ] Publication status tracking
Phase 3 — Professional Workflow
- [ ] Revision history
- [ ] Local backups
- [ ] Import tools
- [ ] Export tools
- [ ] Writing statistics
- [ ] Multi-language interface
- [ ] Additional publishing platforms
- [ ] Platform adapter framework
Future Modules
NovelFlow is intended to grow into a complete professional workspace for serialized-fiction authors.
Future modules may include:
- Series Bible
- Character database
- Relationship tracking
- Worldbuilding
- Timeline management
- Glossary
- Notes
- Research workspace
- AI-assisted editing
- AI writing assistance
- Continuity checking
- Translation workflows
- Localization workflows
- EPUB RAW import
- Side-by-side source and translation editing
Future AI Workspace
A future NovelFlow AI workspace may allow authors to connect AI providers and use project-specific context.
Potential functions include:
- Continue writing from existing chapters
- Rewrite selected passages
- Improve dialogue
- Check grammar
- Check style consistency
- Detect continuity errors
- Compare chapters with a Series Bible
- Detect character inconsistencies
- Detect timeline conflicts
- Maintain terminology
- Analyze manuscript structure
The AI system should operate using relevant project context rather than treating each chapter as an isolated prompt.
Future Translation Workspace
NovelFlow may later include a professional translation and localization workflow.
Example:
┌──────────────────────────────────────────────────────────────┐
│ RAW                    DRAFT                FINAL            │
│                                                              │
│ Original text          AI translation       Edited version   │
│                                                              │
│ 中文原文               English Draft        Final English    │
│                                                              │
└──────────────────────────────────────────────────────────────┘

Potential features:
- EPUB import
- RAW chapter extraction
- Source language detection
- Target language selection
- Translation memory
- Glossary enforcement
- Canon terminology
- Character-name consistency
- Side-by-side editing
- Source comparison
- Missing-content detection
- Localization checks
Klar — hier komplett als eine einzige README.md zum Copy-Paste:
<div align="center">

# NovelFlow

### Write. Organize. Publish.

**A professional desktop writing and publishing studio for web novel authors.**

Built by **Brinkhagen**.

<br>

![Status](https://img.shields.io/badge/status-in%20development-c9a96e)
![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20macOS-blue)
![Desktop](https://img.shields.io/badge/desktop-Electron-47848F)
![Language](https://img.shields.io/badge/UI-multilingual-success)

</div>

---

## About NovelFlow

NovelFlow is a modern desktop workspace designed for authors who publish serialized fiction and web novels.

It combines a distraction-free writing environment, structured book and chapter management, rich-text editing, and publishing tools in one application.

Instead of writing in one application, organizing chapters somewhere else, and manually copying every chapter into a publishing platform, NovelFlow brings the complete workflow into a single workspace.

> Write your story. Organize your chapters. Publish when you're ready.

---

## Core Features

### Professional Writing Editor

Write directly inside NovelFlow using a modern rich-text editor designed for long-form fiction.

Planned editor features include:

- Bold
- Italic
- Underline
- Headings
- Section breaks
- Lists
- Blockquotes
- Text alignment
- Undo / Redo
- Find and Replace
- Word count
- Character count
- Focus mode
- Keyboard shortcuts
- Automatic saving
- Revision history

NovelFlow stores manuscripts in a structured document format so content can later be exported cleanly to different formats and publishing platforms.

---

## Books, Volumes & Chapters

NovelFlow is designed to keep even very large serialized novels organized.

```text
Book
├── Volume 1
│   ├── Chapter 001
│   ├── Chapter 002
│   └── Chapter 003
│
├── Volume 2
│   ├── Chapter 004
│   └── Chapter 005
│
└── Unsorted Drafts

Each chapter can contain its own:
- Title
- Word count
- Notes
- Status
- Last edited date
- Publishing status
- Platform metadata
Chapter Workflow
NovelFlow uses a simple publishing workflow:
Draft
   ↓
Ready
   ↓
Uploaded
   ↓
Published

This makes it easy to see which chapters are still being written, which are ready for review, and which have already been published.
Inkstone / WebNovel Publishing
One of NovelFlow's first publishing integrations is planned for WebNovel Inkstone.
Users authenticate directly with WebNovel through an embedded browser session.
NovelFlow does not need to store the user's WebNovel password.
The publishing workflow is designed around:
- Opening Inkstone inside NovelFlow
- Logging into WebNovel directly
- Selecting ready chapters
- Automatically filling chapter titles
- Transferring chapter content
- Preserving supported formatting
- Saving chapters as drafts
- Reviewing chapters before publication
- Publishing selected chapters
- Tracking local and remote publishing status
Example workflow:
NovelFlow Editor
       ↓
Ready for Publishing
       ↓
Inkstone
       ↓
Upload as Draft
       ↓
Review
       ↓
Publish

Publishing automation is intended to keep authors in control of every release.
Publishing Queue
Authors can prepare multiple chapters before uploading them.
Example:
Chapter	Words	Status
Chapter 021 — The Arrival	2,840	Published
Chapter 022 — The Fleet	3,120	Published
Chapter 023 — The Golden Fleet	2,481	Ready
Chapter 024 — First Contact	3,054	Ready
Chapter 025 — A New Threat	2,910	Draft


Ready chapters can then be processed through the publishing workspace.
Integrated Browser
NovelFlow is being designed as a desktop application with an embedded Chromium environment.
This allows supported publishing platforms to run directly inside NovelFlow while keeping authentication inside the platform's own website.
┌──────────────────────── NovelFlow ────────────────────────┐
│                                                          │
│ Chapters       Writing Editor          Publishing         │
│                                                          │
│ Chapter 23     Your manuscript...      WebNovel ✓         │
│ Chapter 24                              Royal Road         │
│ Chapter 25                              Future Platforms   │
│                                                          │
└──────────────────────────────────────────────────────────┘

The embedded browser is planned to support:
- Persistent local login sessions
- Inkstone navigation
- Chapter editor detection
- Chapter title transfer
- Chapter content transfer
- Draft creation
- Manual review before publishing
- Publishing queue processing
Rich-Text Formatting
NovelFlow is not intended to be a plain-text editor.
The editor is planned to support structured rich-text content including:
- Bold
- Italic
- Underline
- Headings
- Paragraphs
- Lists
- Quotes
- Horizontal separators
- Alignment
- Links
- Supported inline formatting
The editor will use a structured internal document model so formatting can be converted per publishing platform.
Example:
NovelFlow Rich Text
        ↓
Platform Adapter
        ↓
Inkstone-Compatible Content

Unsupported formatting can be simplified safely during publishing without changing the manuscript stored inside NovelFlow.
Multilingual by Design
NovelFlow is designed from the beginning for international authors.
The application architecture separates:
- Interface language
- Book language
- Source language
- Target language
- Publishing language
Example:
Interface Language: German
Book Language: English
Source Language: Chinese
Target Language: English
Publishing Language: English

Initial interface languages are planned to include:
- English
- German
Additional languages can be added through the localization system.
Import & Export
Planned Import Formats
- Markdown
- TXT
- HTML
Planned Export Formats
- Markdown
- TXT
- HTML
- DOCX
- EPUB
Additional formats may be added later.
Platform Integrations
NovelFlow is designed around a modular publishing adapter architecture.
Planned
- WebNovel / Inkstone
Future
- Royal Road
- Scribble Hub
- Additional serialized-fiction platforms
Each publishing integration is separated from the core writing environment.
This allows platform-specific changes to be updated without affecting the entire application.
Desktop Architecture
NovelFlow is planned as a modern cross-platform desktop application.
Core technologies:
Desktop
└── Electron

Interface
├── React
└── TypeScript

Editor
└── Structured Rich Text

Local Application Data
└── SQLite

Publishing
└── Chromium-based platform adapters

Localization
└── i18n

This architecture allows NovelFlow to function locally while leaving room for future cloud synchronization and account-based services.
Privacy & Authentication
NovelFlow is designed so third-party publishing credentials do not need to be stored by NovelFlow.
Where possible, authentication takes place directly inside the publishing platform's own browser environment.
Example:
User
 ↓
Embedded Chromium
 ↓
WebNovel Login
 ↓
Authenticated Local Browser Session

NovelFlow should never require users to provide their publishing password directly to NovelFlow.
Sensitive authentication information must never be committed to this repository.
Product Roadmap
Phase 1 — Writer
- [ ] Desktop application shell
- [ ] User interface
- [ ] Project creation
- [ ] Book management
- [ ] Volume management
- [ ] Chapter management
- [ ] Rich-text editor
- [ ] Autosave
- [ ] Word counting
- [ ] Character counting
- [ ] Chapter status workflow
- [ ] Search
- [ ] Find and Replace
- [ ] Keyboard shortcuts
Phase 2 — Publishing
- [ ] Embedded Chromium browser
- [ ] WebNovel authentication session
- [ ] Inkstone detection
- [ ] Chapter title transfer
- [ ] Chapter content transfer
- [ ] Formatting conversion
- [ ] Draft upload
- [ ] Manual review workflow
- [ ] Publishing queue
- [ ] Publication status tracking
Phase 3 — Professional Workflow
- [ ] Revision history
- [ ] Local backups
- [ ] Import tools
- [ ] Export tools
- [ ] Writing statistics
- [ ] Multi-language interface
- [ ] Additional publishing platforms
- [ ] Platform adapter framework
Future Modules
NovelFlow is intended to grow into a complete professional workspace for serialized-fiction authors.
Future modules may include:
- Series Bible
- Character database
- Relationship tracking
- Worldbuilding
- Timeline management
- Glossary
- Notes
- Research workspace
- AI-assisted editing
- AI writing assistance
- Continuity checking
- Translation workflows
- Localization workflows
- EPUB RAW import
- Side-by-side source and translation editing
Future AI Workspace
A future NovelFlow AI workspace may allow authors to connect AI providers and use project-specific context.
Potential functions include:
- Continue writing from existing chapters
- Rewrite selected passages
- Improve dialogue
- Check grammar
- Check style consistency
- Detect continuity errors
- Compare chapters with a Series Bible
- Detect character inconsistencies
- Detect timeline conflicts
- Maintain terminology
- Analyze manuscript structure
The AI system should operate using relevant project context rather than treating each chapter as an isolated prompt.
Future Translation Workspace
NovelFlow may later include a professional translation and localization workflow.
Example:
┌──────────────────────────────────────────────────────────────┐
│ RAW                    DRAFT                FINAL            │
│                                                              │
│ Original text          AI translation       Edited version   │
│                                                              │
│ 中文原文               English Draft        Final English    │
│                                                              │
└──────────────────────────────────────────────────────────────┘

Potential features:
- EPUB import
- RAW chapter extraction
- Source language detection
- Target language selection
- Translation memory
- Glossary enforcement
- Canon terminology
- Character-name consistency
- Side-by-side editing
- Source comparison
- Missing-content detection
- Localization checks
Planned Application Navigation
NovelFlow
│
├── Dashboard
│
├── Projects
│   └── Books
│       ├── Overview
│       ├── Volumes
│       ├── Chapters
│       └── Drafts
│
├── Library
│
├── Publishing
│   ├── WebNovel
│   └── Future Platforms
│
├── Statistics
│
└── Settings

Future versions may add:
AI Tools
Series Bible
Characters
Worldbuilding
Timeline
Glossary
Translation
Localization

Planned Editor Layout
┌───────────────┬──────────────────────────────────┬───────────────┐
│ Chapters      │ Editor                           │ Chapter Info  │
│               │                                  │               │
│ Volume 1      │ Chapter 23: The Golden Fleet    │ Status        │
│               │                                  │ Ready         │
│ 001           │ Levi stepped onto the bridge... │               │
│ 002           │                                  │ Word Count    │
│ 003           │                                  │ 2,481         │
│ 004           │                                  │               │
│               │                                  │ Notes         │
│               │                                  │ ...           │
└───────────────┴──────────────────────────────────┴───────────────┘

Planned Publishing Workspace
┌───────────────────────────┬─────────────────────────────────────┐
│ Publishing Queue          │ Inkstone Browser                    │
│                           │                                     │
│ ✓ Chapter 23              │ WebNovel / Inkstone                 │
│ ✓ Chapter 24              │                                     │
│ ✓ Chapter 25              │ Chapter Title                       │
│                           │ Chapter Content                     │
│ [Upload as Draft]         │                                     │
│ [Review]                  │                                     │
│ [Publish Selected]        │                                     │
└───────────────────────────┴─────────────────────────────────────┘

Planned Repository Structure
novelflow/
├── apps/
│   └── desktop/
│
├── packages/
│   ├── editor/
│   ├── publishing/
│   ├── database/
│   ├── ui/
│   └── i18n/
│
├── docs/
│   ├── architecture/
│   ├── product/
│   └── publishing/
│
├── assets/
│   ├── branding/
│   └── screenshots/
│
├── README.md
├── SECURITY.md
├── CONTRIBUTING.md
├── CHANGELOG.md
└── ROADMAP.md

Development Status
NovelFlow is currently under active development.

The application is not yet considered production-ready.
Architecture, user interface, publishing integrations and feature scope may change during development.
Security
Security is an important part of NovelFlow's architecture.
Planned principles include:
- No publishing passwords stored by NovelFlow
- Authentication through official platform pages
- Local browser sessions
- Local encrypted application data where appropriate
- No secrets committed to Git
- Strict Electron security configuration
- Context isolation
- Disabled Node.js access for external web content
- Platform adapters separated from the core application
- Safe IPC boundaries
- Input validation
Disclaimer
NovelFlow is an independent software project developed by Brinkhagen.
NovelFlow is not affiliated with, endorsed by, sponsored by, or officially connected to:
- WebNovel
- Inkstone
- Royal Road
- Scribble Hub
- or their respective owners
All third-party names, trademarks, logos and services remain the property of their respective owners.
Developed by Brinkhagen
NovelFlow is developed and maintained by Brinkhagen.
Software. Digital products. Technology.
<div align="center">

NovelFlow
Write. Organize. Publish.
Built by Brinkhagen
© 2026 Brinkhagen. All rights reserved.
</div>
```
