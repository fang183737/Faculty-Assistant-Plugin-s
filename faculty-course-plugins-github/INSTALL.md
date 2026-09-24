Install the Faculty Course Plugins

These instructions assume the Codex or ChatGPT desktop app is already installed. You may install either plugin or both.

## Recommended: install without a terminal

This method uses the Plugins Directory in the desktop app. You do not need to drag files into hidden system folders or type commands.

### 1. Download and extract the repository

1. Open the team repository on GitHub.
2. Select **Code**.
3. Select **Download ZIP**.
4. Open the downloaded ZIP and select **Extract all**.
5. Move the extracted folder to a permanent location, such as Documents.

Do not work from inside the ZIP. Do not move or rename the extracted plugin folder after installation unless you are prepared to repeat the setup.

### 2. Open the correct folder as a Codex project

Open the folder that directly contains both of these items:

```text
.agents/
plugins/
```

If the package was added as `faculty-course-plugins` inside a larger team repository, open the **faculty-course-plugins** subfolder itself as the Codex project. The `.agents` folder must be at the top level of the folder you open.

If Codex asks whether you trust the project, confirm only after verifying that it came from your institution or team.

### 3. Restart the desktop app

Completely close the Codex or ChatGPT desktop app and open it again. Restarting lets the app discover the repository's local plugin marketplace.

### 4. Install from the Plugins Directory

1. Open the **Plugins Directory** in the desktop app.
2. Choose the marketplace named **Faculty Course Plugins**.
3. Open **Rubric Grading Assistant** and select the install or plus button if you want the grading workflow.
4. Open **Canvas Syllabus Assistant** and select the install or plus button if you want the syllabus workflow.

It is fine to install both. They remain separate so instructors can clearly choose the appropriate workflow.

### 5. Start a new task

Start a new Codex task after installation. This lets Codex load the newly installed plugin instructions.

### 6. Test with fictional files

Follow [TESTING.md](TESTING.md) before using real course materials or student work.

## Best option for a larger faculty rollout

A ChatGPT workspace administrator can publish the plugins internally for selected workspace roles. Once published, instructors can find the plugins in the Plugins Directory and select **Install** without downloading a repository, moving folders, or using a terminal.

An administrator can:

1. Install and test the local plugins.
2. Open the ChatGPT Plugins page.
3. Select **Personal**.
4. Open the plugin's three-dot menu.
5. Select **Publish**.
6. Choose which workspace roles should receive access.

Workspace publication keeps the plugins within the organization's workspace; it does not publish them to the public plugin directory.

## Advanced fallback: terminal installation

Use this only if the repository marketplace does not appear automatically or an IT support person is performing the installation.

Open a terminal in the folder containing `.agents` and `plugins`, then run:

```powershell
codex plugin marketplace add .
```

Install the grading plugin:

```powershell
codex plugin add rubric-grading-assistant@faculty-course-plugins
```

Install the syllabus plugin:

```powershell
codex plugin add canvas-syllabus-assistant@faculty-course-plugins
```

Restart the desktop app and start a new task afterward.

## Updating the plugins

For the repository method:

1. Download and extract the newer repository version, or have a team member update the existing folder.
2. Keep the `.agents` and `plugins` folders together.
3. Restart the desktop app.
4. Open the Plugins Directory and reinstall or refresh the affected plugin if prompted.
5. Start a new task.

For workspace-published plugins, the workspace administrator manages the updated version. Instructors should follow the administrator's update notice and start a new task after the update.

## Removing or disabling a plugin

Open the desktop app's plugin management screen and disable or remove the individual plugin. Removing one plugin does not remove the other.

## Why simple drag-and-drop is not recommended

A plugin folder alone is not enough. Codex also needs a marketplace entry that identifies the plugin and its location. Manually placing files into hidden `.codex` or `.agents` folders can overwrite an instructor's existing configuration. The repository marketplace or workspace-published installation methods above are safer.

## Official documentation

See [Package your plugin](https://developers.openai.com/plugins/build/plugins) in the official OpenAI documentation for local marketplace discovery, Plugins Directory installation, and workspace publication.
