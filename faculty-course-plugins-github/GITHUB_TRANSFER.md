# Transfer This Package to GitHub

## Easiest method: GitHub website

1. Create a new, empty GitHub repository.
2. Keep it **Private** until your institution has reviewed the content.
3. Do not ask GitHub to add a README, `.gitignore`, or license during creation; this package already includes the first two.
4. Open the new repository and choose **uploading an existing file**.
5. Upload the contents of this folder, including the `.agents` folder. Upload the contents—not an extra parent folder around them.
6. Commit the upload.
7. Confirm that GitHub shows these paths:
   - `.agents/plugins/marketplace.json`
   - `plugins/rubric-grading-assistant/.codex-plugin/plugin.json`
   - `plugins/canvas-syllabus-assistant/.codex-plugin/plugin.json`
8. Add a license only after the repository owner has selected one.
9. Test a fresh download using [INSTALL.md](INSTALL.md).

If the browser does not preserve empty or hidden-looking folders, use GitHub Desktop instead.

## GitHub Desktop method

1. Open GitHub Desktop.
2. Choose **File > Add Local Repository** and select this folder.
3. If prompted, choose **create a repository here**.
4. Review the files before the first commit. Course records and real student work must not be present.
5. Commit the files with a message such as `Initial faculty plugin package`.
6. Choose **Publish repository** and keep it private during review.

## Command-line method

From this repository root:

```powershell
git init
git add .
git commit -m "Initial faculty plugin package"
git branch -M main
git remote add origin https://github.com/ORGANIZATION/REPOSITORY.git
git push -u origin main
```

Replace `ORGANIZATION` and `REPOSITORY` with the actual GitHub location.

## Before every public release

- Confirm no student data, course records, tokens, local paths, or personal identifiers are included.
- Run both plugin validators and both fictional workflow tests.
- Update plugin versions when behavior changes.
- Review the Word guides and Markdown instructions for accuracy.
- Decide whether the repository needs a license, support contact, privacy notice, or institutional disclaimer.
