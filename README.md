# PhpStorm Event-Stream Project

## What is Git? (Introduction to Git)
Git is a Distributed Version Control System (DVCS) that helps developers manage their codebase by tracking changes, collaborating, and maintaining a history of the project.

### Why Use Git?
- **Version Tracking**: Git keeps track of every change made to files in a project. You can revert to previous versions if something goes wrong.
- **Collaboration**: Multiple developers can work on the same project simultaneously without overwriting each other's work.
- **Backup**: Changes are safely stored, and you can upload your code to a remote repository (e.g., GitHub or GitLab).
- **Conflict Resolution**: When two people modify the same file, Git highlights the conflict so it can be resolved before merging changes.

### Common Git Terms
- **Repository (Repo)**: A directory containing your project and the `.git` folder, which stores version history and metadata.
- **Commit**: A snapshot of changes saved to your local repository.
- **Branch**: A separate workspace to work on features or bug fixes without disturbing the main codebase.
- **Merge**: Combining changes from different branches.
- **Pull**: Download changes from a remote repository.
- **Push**: Upload your commits to a remote repository.

---

## Setting Up Git in PhpStorm

### Install Git on Your Machine
1. Download Git from [https://git-scm.com/](https://git-scm.com/) and install it.
2. Follow the installation instructions for your operating system.

### Configure Git in PhpStorm
1. Open PhpStorm.
2. Navigate to **File > Settings > Version Control > Git** (or **PhpStorm > Preferences > Version Control > Git** on macOS).
3. Locate the field for **Path to Git executable**:
   - Example (Windows): `C:\Program Files\Git\bin\git.exe`
   - Example (macOS/Linux): `/usr/bin/git`
4. Click **Test** to ensure Git is detected. You’ll see a success message if the setup is correct.
5. Click **OK** to save your settings.

---

## Getting Started with a Git Repository

### Option A: Create a New Repository
1. Open your project in PhpStorm.
2. Go to the top menu and click **VCS > Enable Version Control Integration**.
3. In the pop-up window, select **Git** from the dropdown menu and click **OK**. This initializes a Git repository in your project folder.
4. Your project is now under version control. PhpStorm will track changes automatically.

### Option B: Clone an Existing Repository
1. Click **VCS > Get from Version Control**.
2. In the dialog box, select **Git** as the version control type.
3. Paste the repository URL (e.g., `https://github.com/your-username/repo-name.git`) in the **URL** field.
4. Choose a local directory where you want the project to be stored, then click **Clone**.
5. PhpStorm will download the repository and open it.

---

## Using Git Features in PhpStorm

### Commit Changes
1. After editing files, open the Commit tool:
   - Click the **Git** tab at the bottom of the IDE, or
   - Go to **VCS > Commit**, or
   - Use the shortcut **Ctrl + K** (Windows/Linux) or **Cmd + K** (macOS).
2. In the **Commit Changes** dialog:
   - Check the files you want to include in the commit.
   - Write a commit message describing your changes.
3. Click **Commit** to save the changes locally.

### Push Changes to GitHub
1. After committing, click **VCS > Git > Push** (or press **Ctrl + Shift + K** on Windows/Linux, **Cmd + Shift + K** on macOS).
2. Review the changes to push and click **Push**.
3. The changes will be uploaded to the GitHub repository.

### Pull Changes from GitHub
1. Click **VCS > Git > Pull**.
2. PhpStorm will download changes from the remote repository and merge them into your local branch.

---

## Creating and Managing Branches in PhpStorm

### Create a New Branch
1. Click the **Git: Main** option in the bottom-right corner of the IDE.
2. Select **New Branch** from the menu.
3. Enter a branch name (e.g., `feature-login`) and click **Create**.

### Switch Branches
1. Click the current branch name in the bottom-right corner.
2. Select the branch you want to switch to.

### Merge Branches
1. Switch to the branch you want to merge into (e.g., `main`).
2. Click **VCS > Git > Merge Changes**.
3. Select the branch to merge.

---

## Collaborating with Team Members

### Share the Repository
1. Go to the GitHub repository page.
2. Invite your teammates as collaborators:
   - Click **Settings > Collaborators > Add**.
3. Send them the repository URL to clone.

### Avoid Conflicts
1. Assign specific branches or tasks to team members.
2. Regularly pull changes from GitHub before starting work:
   - **VCS > Git > Pull**.

### Use Pull Requests on GitHub
1. After completing work on a branch, push the branch to GitHub.
2. Go to the repository page and click **Pull Requests > New Pull Request**.
3. Compare the branch with `main` and create the PR for teammates to review.

---

## Install Node.js Modules
1. Ensure `package.json` is included in the repository.
2. Navigate to the project folder in the terminal.
3. Run the following command to install dependencies:
   ```bash
   npm install
