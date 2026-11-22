# CognoCraft Studio

A zero-dependency, browser-based rapid authoring studio for Instructional Designers building interactive HTML5 and SCORM 1.2 learning blocks for **Articulate Rise 360** and enterprise LMS platforms.

## Key Capabilities

* **16 Pedagogy-Aligned Interactive Blocks:** Mapped to **Bloom’s Taxonomy** and **Gagné’s Nine Events of Instruction**:
  * *Scenarios & Decisions:* Chat Scenario, Scenario Walkthrough, Scenario Judgment Card
  * *Processes & Concepts:* Process Flow, Interactive Timeline, Concept Breakdown
  * *Practice & Assessment:* Diagnostic Quiz Block, Active Recall Flashcards, Fill in the Blank, Sequencing Activity, Category Sorting
  * *Visual & Reflection:* Hotspot / Label the Diagram (with click-to-place percentage pins & Explore/Quiz modes), Before / After Slider, Annotated Visual Carousel, Reflective Journal, Interactive Readiness Checklist
* **100% White-Labeled Output:** Generates clean, unbranded single-file HTML5 bundles with zero external watermarks or tool branding.
* **Articulate Rise 360 & SCORM 1.2 Integration:**
  * Automatically injects `window.parent.postMessage({ type: 'complete' }, '*')` to unlock Rise 360 **Continue** blocks upon completion.
  * Includes dynamic `ResizeObserver` iframe auto-resizing to prevent double scrollbars.
  * 1-click **SCORM 1.2 (`.zip`)** micro-package export (`imsmanifest.xml` + SCORM 1.2 runtime API wrapper).
* **AI-Ready SME Content Generator & Review Scripts:**
  * Generates block-specific JSON schema prompts to convert raw Subject Matter Expert (SME) notes via any LLM.
  * Exports 5-column **SME Review Tables** (`.doc` and `.html`) for stakeholder redlining and sign-off.
* **No-Code Visual HTML Editor & Brand Kits:**
  * Click directly on preview headings, paragraphs, or buttons to edit text, bold keywords, or globally replace hex brand colors without touching code.
  * Save/load reusable **Brand Kits** and `.json` / `.html` project snapshots for post-launch edits.

## Running Locally or Deploying

Because **CognoCraft Studio** is built as a self-contained single-file web application:

1. **Run Locally:** Open `index.html` directly in any modern browser (Chrome, Edge, Firefox, Safari)—no build step or Node.js server required.
2. **Host on GitHub Pages:**
   * Go to your repository **Settings → Pages**.
   * Under **Build and deployment**, set **Source** to `Deploy from a branch`, select `main` and `/ (root)`, and click **Save**.
