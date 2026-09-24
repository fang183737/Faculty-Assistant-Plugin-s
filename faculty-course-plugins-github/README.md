# Faculty Course Plugins

This repository contains two separate, local Codex plugins for instructors:

- **Rubric Grading Assistant** drafts rubric-based scoring analysis and feedback for one submission at a time.
- **Canvas Syllabus Assistant** revises a syllabus and prepares accessible content for manual transfer into Canvas.

The plugins are intentionally separate so instructors can install only the workflow they need. Neither plugin publishes to Canvas or makes a final academic decision on the instructor's behalf.

## Start here

1. Read [INSTALL.md](INSTALL.md) to install the local marketplace and either plugin.
2. Open [docs/Faculty Plugin Usage Guide.docx](docs/Faculty%20Plugin%20Usage%20Guide.docx) for copy-ready prompts and review checklists.
3. Open [docs/Faculty Plugin Customization Guide.docx](docs/Faculty%20Plugin%20Customization%20Guide.docx) before adapting a plugin to a course.
4. Use [TESTING.md](TESTING.md) and the fictional files in `test-fixtures/` before working with real course materials.

## Repository contents

```text
faculty-course-plugins/
├── .agents/plugins/marketplace.json
├── plugins/
│   ├── rubric-grading-assistant/
│   └── canvas-syllabus-assistant/
├── docs/
├── test-fixtures/
├── INSTALL.md
├── CUSTOMIZE.md
├── TESTING.md
└── GITHUB_TRANSFER.md
```

## Important safeguards

- Use only institution-approved AI tools and accounts for student information.
- Remove student identifiers whenever possible.
- Keep original files unchanged and treat generated work as a draft.
- An instructor must approve every score, feedback message, policy change, and date.
- The grading plugin must not determine AI use, plagiarism, or misconduct.
- The syllabus plugin prepares content for manual transfer; it does not publish to Canvas.

## License decision before public release

This repository does not select a software license for you. Before making a GitHub repository public, have the repository owner choose and add an appropriate `LICENSE` file.
