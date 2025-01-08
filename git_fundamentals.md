# Fundamentals of GitHub and VS Code

## GitHub Fundamentals

### 1. What is GitHub?
- **Definition**: A cloud-based platform for version control and collaboration using Git.
- **Purpose**: Helps manage code repositories, track changes, and collaborate on projects.

### 2. Key GitHub Concepts
- **Repository**: A storage space for your project, including code, files, and history.
- **Commit**: A snapshot of your code at a specific point in time.
- **Branch**: A parallel version of your repository to work on features without affecting the main branch.
- **Pull Request (PR)**: A way to propose and collaborate on changes before merging into the main branch.
- **Merge**: Integrating changes from one branch into another.
- **Issues**: A feature to track bugs, features, or tasks in your project.
- **GitHub Pages**: Hosting static websites directly from a repository.

### 3. GitHub Workflow
1. **Clone a Repository**: Copy a remote repository to your local machine.
2. **Make Changes**: Edit code or files locally.
3. **Stage Changes**: Use `git add` to stage files for commit.
4. **Commit Changes**: Save a snapshot of your changes (`git commit`).
5. **Push Changes**: Upload your changes to the remote repository (`git push`).
6. **Collaborate**: Create pull requests, review code, and merge changes.

### 4. Key Git Commands
- **`git clone`**: Clone a repository to your local machine.
- **`git add <file>`**: Stage a file for commit.
- **`git commit -m "message"`**: Commit changes with a message.
- **`git push`**: Push commits to a remote repository.
- **`git pull`**: Fetch and merge changes from the remote repository.
- **`git status`**: Check the status of your working directory.

### 5. GitHub Features to Explore
- **Forking**: Creating a copy of someone else’s repository to work on.
- **GitHub Actions**: Automating workflows like testing and deployment.
- **Markdown**: Writing README files and documentation.

---

## VS Code Fundamentals

### 1. What is Visual Studio Code (VS Code)?
- **Definition**: A lightweight, extensible code editor with built-in support for debugging, Git, and extensions.
- **Purpose**: Enhances productivity with features like IntelliSense, terminal integration, and extensions.

### 2. Key VS Code Features
- **Command Palette**: Access commands and shortcuts with `Ctrl+Shift+P` (Windows/Linux) or `Cmd+Shift+P` (Mac).
- **Integrated Terminal**: Use Git, npm, or other tools directly in the editor.
- **Extensions**: Add functionality (e.g., Prettier, ESLint, Live Server).
- **Debugger**: Step through your code to identify and fix bugs.
- **Code Navigation**: Quickly jump between files, methods, or variables.

### 3. Setting Up VS Code
1. **Install Extensions**:
   - **GitLens**: Enhances Git capabilities.
   - **Prettier**: Automatically formats code.
   - **Live Server**: For real-time preview of web projects.
   - **Bracket Pair Colorizer**: Makes matching brackets easier to identify.
2. **Set Up Git**:
   - Link your GitHub account in VS Code.
   - Use the source control panel for Git commands.
3. **Customizing Settings**:
   - Adjust themes, fonts, and keybindings.
   - Configure workspace-specific settings.

### 4. Git in VS Code
- **Source Control Panel**:
  - Stage, commit, and push changes directly from VS Code.
  - View the change history for each file.
- **Built-in Git Commands**:
  - Use the integrated terminal to run Git commands.
  - Resolve merge conflicts with VS Code’s UI tools.

### 5. Debugging Basics
- **Set Breakpoints**: Pause your code at specific lines.
- **Run and Debug**: Start debugging sessions for your project.
- **Inspect Variables**: Monitor variable values during runtime.

### 6. Best Practices
- **Workspace Organization**: Keep your project folder clean and structured.
- **Use Version Control**: Commit changes regularly with meaningful messages.
- **Write Good Documentation**: Use Markdown for README files and comments.

---

## Suggested Workflow for Students

### 1. Initialize a Project
- Create a local project folder and initialize a Git repository (`git init`).
- Create a new repository on GitHub and connect it to your local repository.

### 2. Work on Code
- Open your project in VS Code.
- Use extensions like Live Server to preview changes in real time.

### 3. Version Control
- Stage, commit, and push changes regularly.
- Create branches for new features or experiments.

### 4. Collaboration
- Use pull requests for peer code reviews.
- Track issues and assign tasks using GitHub.

---

## Resources for Learning
- [GitHub Docs](https://docs.github.com/)
- [VS Code Docs](https://code.visualstudio.com/docs)
- [Pro Git Book](https://git-scm.com/book/en/v2)
- [GitHub Learning Lab](https://lab.github.com/)
- [YouTube Tutorials](https://www.youtube.com/) (Search for GitHub and VS Code Basics)

---

## Hands-On Exercises
1. **Create a GitHub Repository**:
   - Create a new repository and clone it to your local machine.
2. **Make and Push Changes**:
   - Edit a file in VS Code, stage it, commit, and push to GitHub.
3. **Collaborate with a Peer**:
   - Fork and clone each other’s repositories.
   - Submit pull requests and merge changes.
4. **Host a Website with GitHub Pages**:
   - Build a simple HTML/CSS project and deploy it using GitHub Pages.
5. **Debug a Project in VS Code**:
   - Use breakpoints and the debugger to fix errors in a JavaScript file.

---

### Notes for Instructors
- Focus on practical exercises to reinforce concepts.
- Encourage students to document their projects in Markdown.
- Assign group projects to simulate real-world collaboration using GitHub.
