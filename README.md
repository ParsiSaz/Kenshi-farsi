<div align="center">

# ⚔️ Kenshi | Persian Localization (پارسی‌ساز کنشی)
### *Official ParsiSaz Community Translation, Custom Font Atlas & Localization Package*

<br/>

[![ParsiSaz Portal](https://img.shields.io/badge/🌐_Documentation_Portal-parsisaz.github.io%2Fparsisaz-00f2fe?style=for-the-badge&logo=googlechrome)](https://parsisaz.github.io/parsisaz/)
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg?style=for-the-badge)](https://www.gnu.org/licenses/gpl-3.0)
[![Locale](https://img.shields.io/badge/Locale-fa__IR-emerald?style=for-the-badge)](#-project-structure)
[![Maintainer](https://img.shields.io/badge/Maintained_by-Danial_Pahlavan-blue?style=for-the-badge&logo=github)](https://github.com/DanialPahlavan)

</div>

---

## 📖 Overview
This repository contains the Persian localization patch for **Kenshi** (by Lo-Fi Games), following the **ParsiSaz 2026 Game Localization Architecture (L10N-STD-2026)**.

### ⚙️ Engine Technical Obstacles
1. **Engine Limitations**: The OGRE-based engine lacks native Right-to-Left (RTL) HarfBuzz-style text shaping, rendering non-reshaped words in reverse order.
2. **Alphabet & Glyph Support**: Standard font atlases omit Arabic/Persian Unicode ranges; required injecting a customized TTF with predefined Unicode codepages.
3. **Word Disconnection**: Engine string renderers isolate cursive Persian characters without dedicated joiner glyph substitutions.

---

## 🗂️ Project Structure (L10N-STD-2026)

```
Kenshi-farsi/
├── locale/fa_IR/               # BCP-47 Persian Localization Catalog
│   ├── LC_MESSAGES/
│   │   ├── main.po             # Editable translation strings
│   │   ├── main.mo             # Compiled high-performance binary catalog
│   │   └── main.pot            # Master extraction template
│   ├── dialogue/               # Translated character dialog trees
│   └── gui/                    # UI, inventory, and HUD strings
├── HISTORY.md                  # Semantic Version Changelog
├── README.md                   # Project documentation
└── LICENSE                     # GNU General Public License v3
```

---

## 🚀 Installation Instructions

1. Download `fa_IR.zip` from the [Latest Releases](https://github.com/ParsiSaz/Kenshi-farsi/releases).
2. Extract the archive into your game directory under:
   ```text
   <Kenshi_Installation_Folder>/locale/fa_IR/
   ```
3. Launch Kenshi. In the launcher settings, choose **`fa_IR`** from the language dropdown list.
4. Start the game. All dialogues, items, and UI elements will be displayed in Persian.

---

## 🌐 Central Documentation & Bug Reports
For more details on engine hurdles, reverse engineering, and other games in the ecosystem:
👉 **[Open ParsiSaz Live Portal](https://parsisaz.github.io/parsisaz/)**
