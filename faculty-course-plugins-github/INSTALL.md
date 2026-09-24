# Install the Faculty Course Plugins

These instructions assume Codex is already installed. You can install either plugin or both.

## 1. Download the repository

Choose one method:

- **GitHub website:** Select **Code**, select **Download ZIP**, and extract the ZIP to a permanent folder.
- **Git:** Clone the repository to a permanent folder on the computer.

Do not install from inside the downloaded ZIP. Extract it first, and do not move or rename the folder after installation unless you repeat the marketplace setup.

## 2. Open a terminal in the repository folder

In Windows File Explorer, open the extracted repository folder, right-click an empty area, and choose **Open in Terminal**.

## 3. Add the local marketplace

Run this command from the repository root:

```powershell
codex plugin marketplace add .
```

The marketplace name is `faculty-course-plugins`.

## 4. Install the plugin or plugins you want

Rubric grading:

```powershell
codex plugin add rubric-grading-assistant@faculty-course-plugins
```

Canvas syllabus revision:

```powershell
codex plugin add canvas-syllabus-assistant@faculty-course-plugins
```

It is fine to install both. Each plugin has a separate purpose and name.

## 5. Start a new Codex task

Close the installation task and start a new task. This lets Codex load the newly installed plugin instructions.

## 6. Test with fictional files

Follow [TESTING.md](TESTING.md) before using real course materials.

## Updating after downloading a newer repository version

1. Replace or update the local repository folder.
2. Open a terminal in the repository root.
3. Re-run the applicable `codex plugin add` command above.
4. Start a new Codex task.

If Codex continues to use an older version, ask the repository maintainer to update the plugin version or development cachebuster before reinstalling.

## Removing a plugin

Use Codex's plugin management screen, or run the appropriate Codex plugin removal command supported by your installed Codex version. Removing one plugin does not remove the other.
