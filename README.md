
# GTU Important Questions — Claude AI Skill

A Claude AI skill for analyzing Gujarat Technological University (GTU) previous-year question papers and generating a unit-wise important questions PDF for exam preparation.

## Overview

Students often need to review multiple previous-year question papers to identify recurring questions, understand examination patterns, and prioritize topics from their syllabus.

**GTU Important Questions** helps automate this process using Claude AI. It analyzes uploaded question papers alongside the subject syllabus and organizes questions into a structured revision guide.

## Features

- **Unit-wise classification:** Organizes questions according to the provided subject syllabus.
- **Frequency analysis:** Identifies questions repeated across multiple examination papers.
- **Marks tracking:** Records marks wherever they are available in the source papers.
- **Exam session tracking:** Records the examination sessions in which questions appeared.
- **Priority labels:** Categorizes questions using MUST DO, HIGH, MEDIUM, LOW, and NEW labels.
- **Similar question grouping:** Groups related questions while preserving their meaning.
- **Consolidated revision list:** Creates a focused list of important questions.
- **PDF output:** Aims to generate a clean, print-friendly A4 PDF for revision.
- **Question-focused analysis:** Concentrates on identifying and prioritizing questions rather than writing answers.

## How It Works

1. Upload the relevant GTU Summer and Winter previous-year question papers.
2. Upload the official syllabus for the subject.
3. Ask Claude to analyze the documents using the `analyze-paper` skill.
4. The skill extracts questions and maps them to syllabus units.
5. Claude analyzes question frequency, marks, and examination sessions.
6. Questions are grouped and prioritized according to the skill instructions.
7. Review the analysis and use the generated PDF for revision.

## Priority Levels

| Priority | Frequency guideline |
|---|---|
| MUST DO | 5 or more appearances |
| HIGH | 3–4 appearances |
| MEDIUM | 2 appearances |
| LOW | 1 appearance |
| NEW | Potentially new topic, when supported by available evidence |

The frequency thresholds above describe the intended classification rules. Check `skills/analyze-paper/SKILL.md` for the actual instructions used by the current version.

The NEW label is separate from frequency-based categories and should not be assigned without sufficient evidence.

## Repository Structure

```text
gtu-important-questions-claude-skill/
├── .claude-plugin/
│   └── plugin.json
├── skills/
│   └── analyze-paper/
│       └── SKILL.md
├── README.md
└── LICENSE
```

A marketplace manifest can also be included when configuring Claude Code marketplace distribution.

## Installation and Usage

### Using Claude.ai

1. Obtain the skill package from this repository.
2. Follow the custom-skill import instructions available in your Claude interface.
3. Upload the subject syllabus and relevant question papers.
4. Ask Claude to analyze the papers and produce the important questions report.

Custom-skill availability and PDF-generation capabilities depend on your Claude account and environment.

### Using Claude Code

This project is designed for a Claude Code skill/plugin workflow.

For marketplace installation, the repository must have a valid marketplace manifest and plugin configuration.

Follow the official documentation:

https://docs.anthropic.com/en/docs/claude-code/plugins

## Limitations

- Analysis quality depends on the completeness and readability of the uploaded documents.
- Scanned question papers may require OCR, and extracted text should be verified.
- Missing marks, dates, and examination sessions must not be invented.
- Similar questions should be checked before being merged.
- Historical question frequency does not guarantee future examination questions.
- Always compare the final analysis with the original papers.
- PDF output depends on the file-generation tools available in the execution environment.

## Contributing

Suggestions, corrections, and improvements are welcome.

1. Fork the repository.
2. Make your changes in a separate branch.
3. Submit a pull request describing your improvements.

Please test proposed changes against representative question papers and syllabi.

## Disclaimer

This is an independent, community-created educational project. It is not affiliated with, endorsed by, or officially associated with Gujarat Technological University (GTU), Anthropic, or Claude.

GTU is referenced solely to describe the intended educational use case.

This project supports exam preparation and does not guarantee examination results or predict future question papers.

## License

This project is distributed under the MIT License. See the [LICENSE](LICENSE) file for details.
