# Customize the Plugins for a Course

Make a copy or a Git branch before editing. Keep each plugin focused on its existing workflow.

## Rubric Grading Assistant

Edit files under:

```text
plugins/rubric-grading-assistant/skills/rubric-grading/
```

Useful locations:

- `SKILL.md` contains the workflow and boundaries.
- `assets/grading-report-template.md` controls the suggested report structure.
- `references/calibration.md` contains scoring calibration guidance.
- `references/privacy-and-grading-safety.md` contains privacy and academic-decision safeguards.

Appropriate course-specific additions include the rubric scale, rounding rule, authorized late-work policy, feedback tone, and required report sections. Do not add student records, completed student submissions, passwords, or access tokens to the plugin.

## Canvas Syllabus Assistant

Edit files under:

```text
plugins/canvas-syllabus-assistant/skills/syllabus-canvas/
```

Useful locations:

- `SKILL.md` contains the workflow and boundaries.
- `assets/change-log-template.md` controls the change-log structure.
- `references/accessibility-checklist.md` contains the accessibility review.
- `references/canvas-handoff.md` contains the manual Canvas transfer guidance.

Appropriate course-specific additions include required syllabus sections, approved policy sources, date-checking rules, department wording, and Canvas formatting preferences. Do not hard-code term dates that will become stale without also documenting when and how to update them.

## After making changes

1. Update the plugin version in its `.codex-plugin/plugin.json` when releasing a meaningful change.
2. Run the validation commands in [TESTING.md](TESTING.md).
3. Reinstall the changed plugin.
4. Start a new Codex task.
5. Test with fictional files before using live course material.

The Word customization guide in `docs/` provides a nontechnical, step-by-step version of this process.
