
<div align="center">

# 🎓 GTU Important Questions

### Claude AI Skill for Smarter Exam Preparation

Analyze GTU previous-year question papers, discover recurring questions, prioritize revision, and generate a structured important-questions PDF.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/Platform-Claude%20AI-blueviolet)](https://claude.ai/)
[![University](https://img.shields.io/badge/University-GTU-orange)](https://www.gtu.ac.in/)
[![Status](https://img.shields.io/badge/Status-Community%20Project-success)](https://github.com/KrishSardhara013/gtu-important-questions-claude-skill)

**Less time searching. More focused revision.**

[Getting Started](#-getting-started) •
[Features](#-features) •
[Installation](#-claude-code-plugin-installation) •
[Contributing](#-contributing)

</div>

---

## 📌 Overview

Preparing for university examinations often means reviewing multiple previous-year question papers, comparing repeated questions, tracking marks, and mapping everything to the syllabus.

**GTU Important Questions** is a Claude AI skill designed to simplify this process for students of Gujarat Technological University (GTU).

Provide your subject syllabus and previous-year question papers, and use Claude to organize questions unit-wise, analyze repetition patterns, assign revision priorities, and create a consolidated PDF.

> Turn scattered question papers into a structured revision guide.

## ✨ Features

| Feature | Description |
|---|---|
| 📚 Unit-wise Classification | Maps questions to units in the provided syllabus |
| 🔁 Frequency Analysis | Identifies recurring questions across uploaded papers |
| 📝 Marks Tracking | Records question marks when available |
| 📅 Exam Session Tracking | Tracks the sessions in which questions appeared |
| 🎯 Priority Labels | Organizes questions into revision priority categories |
| 🔗 Similar Question Grouping | Groups related questions while preserving their meaning |
| 📄 PDF Generation | Produces a printable revision document when supported by the environment |
| 🎓 Exam-Focused Workflow | Focuses on question analysis rather than generating answers |

## ⚙️ How It Works

```text
Upload Previous-Year Papers
            +
      Upload Syllabus
            ↓
    Claude AI Analysis
            ↓
   Extract and Organize
        Questions
            ↓
  Map Questions to Units
            ↓
 Analyze Frequency and Marks
            ↓
  Assign Priority Labels
            ↓
 Consolidated Important
       Questions PDF
```

### Getting started

1. Collect the available GTU Summer and Winter question papers for your subject.
2. Obtain the official subject syllabus.
3. Open Claude in an environment where the skill is available.
4. Upload the documents and ask Claude to analyze them using `analyze-paper`.
5. Review the unit mapping, repeated questions, and priority classifications.
6. Generate and verify the final revision PDF.

## 🎯 Priority Classification

The skill is intended to organize questions using frequency-based priorities.

| Priority | Intended frequency | Suggested use |
|---|---:|---|
| 🔴 MUST DO | 5+ appearances | Highest revision priority |
| 🟠 HIGH | 3–4 appearances | Important recurring questions |
| 🔵 MEDIUM | 2 appearances | Include in revision |
| ⚪ LOW | 1 appearance | Review if time permits |
| 🆕 NEW | Requires supporting evidence | Investigate potentially new topics |

**Important:** These thresholds describe the intended classification scheme. Refer to `skills/analyze-paper/SKILL.md` for the exact rules implemented by the current version.

The NEW label is separate from frequency-based priorities. A topic should only be labeled new when the available papers support that conclusion.

## 🧰 Requirements

- A Claude account and access to the relevant Claude skill or plugin workflow.
- Subject syllabus in a readable document format.
- Previous-year question papers in readable PDFs or other supported formats.
- PDF generation capability in the selected execution environment.

Scanned documents may require OCR. Check extracted questions and marks against the originals.

## 🚀 Claude Code Plugin Installation

This repository is intended to be distributed as a Claude Code plugin.

### Prerequisites

- Claude Code installed and working.
- A public GitHub repository.
- A valid `.claude-plugin/plugin.json`.
- A valid `.claude-plugin/marketplace.json` configured to reference this plugin.

### Step 1 — Add the marketplace

Open Claude Code and enter:

```text
/plugin marketplace add KrishSardhara013/gtu-important-questions-claude-skill
```

This registers the repository as a plugin marketplace. It does not install the plugin by itself.

### Step 2 — Install the plugin

Enter:

```text
/plugin install gtu-important-questions@gtu-study-tools
```

The plugin name and marketplace name must match the values in your committed configuration files.

### Step 3 — Activate the plugin

Follow the installation prompts and select the desired installation scope. If Claude Code asks you to reload plugins, run:

```text
/reload-plugins
```

### Step 4 — Use the skill

Upload your subject syllabus and question papers, then ask Claude to analyze them using the `analyze-paper` skill.

**Installation note:** These commands assume the marketplace manifest and plugin metadata have been validated. If installation fails, check the marketplace name, plugin name, repository structure, and Claude Code's error message.

Official documentation:

- [Claude Code Plugins](https://docs.anthropic.com/en/docs/claude-code/plugins)
- [Plugin Marketplaces](https://docs.anthropic.com/en/docs/claude-code/plugin-marketplaces)

## 📁 Repository Structure

```text
gtu-important-questions-claude-skill/
├── .claude-plugin/
│   ├── plugin.json
│   └── marketplace.json
├── skills/
│   └── analyze-paper/
│       └── SKILL.md
├── README.md
└── LICENSE
```

## ⚠️ Limitations

- Results depend on the quality and completeness of the uploaded documents.
- OCR or text extraction can introduce errors.
- Missing marks, dates, and examination sessions should not be invented.
- Similar questions may need manual verification before being grouped.
- Historical frequency does not guarantee future examination questions.
- Generated PDFs should be checked against the original source documents.
- Actual PDF generation depends on the capabilities of the environment running Claude.

## 🛣️ Future Improvements

Potential future enhancements include:

- Better handling of scanned question papers.
- Improved duplicate and paraphrased question detection.
- More detailed frequency summaries by examination session.
- Additional PDF formatting options.
- Broader syllabus formats and support for more subjects.

These are possible future enhancements, not promises of existing functionality.

## 🤝 Contributing

Contributions, bug reports, and suggestions are welcome.

1. Fork the repository.
2. Create a branch for your changes.
3. Make your changes and test them with representative question papers.
4. Submit a pull request describing the improvement.

Please avoid submitting private documents or copyrighted examination papers without permission to redistribute them.

## 📜 License

This project is licensed under the [MIT License](LICENSE).

You may use, modify, and redistribute the project subject to the terms of that license.

## ⚖️ Disclaimer

This is an independent, community-created educational project. It is not affiliated with, endorsed by, or officially associated with Gujarat Technological University (GTU), Anthropic, or Claude.

GTU is mentioned only to describe the intended educational use case.

This tool is intended to support exam preparation. It does not guarantee examination results or predict future question papers.

---

<div align="center">

**Built to make exam preparation more organized.**

Created by [KrishSardhara013](https://github.com/KrishSardhara013)

⭐ If you find this project useful, consider starring the repository!

</div>
