# useful__little_things
> *Tools that are useful, but simple.*

---

## 🛠️ Included Tools

| Tool | Status | Type | Description |
| :--- | :---: | :---: | :--- |
| **[📄 PDF Instant Translator & Vocab Ledger](./pdf-instant-translator)** | `v1.0.0` | Standalone Web App (`.html`) | 1-click zero-latency foreign language PDF reader with sub-pixel word alignment & auto vocab ledger. |

---

## 📑 Tool Details

### 1. [PDF Instant Translator & Vocab Ledger](./pdf-instant-translator)
A zero-install, single-file browser application engineered to read and translate dense foreign-language academic PDFs with surgical precision.

* **The Problem It Solves**: Default web PDF viewers rely on browser DOM text selection layers. Due to proportional font tracking and kerning mismatches, clicking a single word frequently captures adjacent characters or fragments (e.g. clicking `lament` incorrectly grabs `consistently`).
* **The Engineering Fix**: Replaces DOM selection overlays with a **deterministic glyph advance reconstruction engine** that parses low-level PDF operator streams (`OPS.showText`) directly from embedded fonts, achieving **100% click resolution accuracy (1.39 px mean boundary error)**.
* **Key Capabilities**:
  - 🎯 **1-Click Lookup**: Hover to highlight, single click to show an instant glassmorphic translation tooltip.
  - 🖱️ **True Drag Selection**: Sweep across phrases or lines with smooth highlight merging.
  - 📚 **Integrated Vocabulary Ledger**: Automatically logs lookups with timestamps; supports live search, filtering, and `.txt` export.
  - 📖 **Kindle-Style Reader Mode**: Instant toggle between high-res PDF canvas and clean, legible eBook text.
  - 📦 **100% Standalone**: Single `.html` file with zero build step, zero backend, and zero local dependencies.

👉 **[Read Full Engineering Case Study & Technical Documentation](./pdf-instant-translator/README.md)**
