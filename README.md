# SE Git Homework

A simple Software Engineering project for practicing Python programming, Git version control, and collaboration through GitHub.

## Project Files

- `hello.py` — Hello World program.
- `apple.py` — Additional Python script.
- `README.md` — Project overview and instructions.

## Setup

1. Install Python 3 and Git.
2. Clone this repository using its GitHub URL:
   ```bash
   git clone <repository-url>
   ```
3. Open the project folder in VS Code or another editor.

## Running the Programs

Open a terminal in the project folder and run:

```bash
python hello.py
python apple.py
```

## Working with Branches

Branches let you develop changes separately from the main version of the project.

Before starting, update your local `main` branch and create a branch for your work:

```bash
git switch main
git pull origin main
git switch -c feature/update-hello
```

After editing your files, save your changes in a commit and push your branch to GitHub:

```bash
git add hello.py
git commit -m "Update Hello World program"
git push -u origin feature/update-hello
```

Use a descriptive branch name, such as `feature/add-greeting` or `fix/input-error`. Replace the example file and branch names with those for your changes.

## Pull Requests

A pull request proposes merging changes from your branch into `main` and gives teammates a chance to review them.

1. Push your branch to GitHub.
2. Open the repository and select **Compare & pull request**.
3. Set `main` as the base branch and your working branch as the compare branch.
4. Add a title and description explaining what changed and how you tested it.
5. Request a teammate's review.
6. Address feedback by committing and pushing updates to the same branch.
7. Merge once the changes are approved and required checks pass.

After merging, update your local copy:

```bash
git switch main
git pull origin main
```

## Collaboration

- Use GitHub Issues to report bugs, suggest improvements, and assign tasks.
- Agree on who will work on each task to avoid duplicate work.
- Create a separate branch for each feature or fix.
- Write clear commit messages that explain your changes.
- Keep pull requests small so they are easy to review.
- Review teammates' code and give constructive feedback.
- Run the affected programs before requesting review or merging.

### Handling Merge Conflicts

A merge conflict happens when Git cannot automatically combine changes.

To bring the latest `main` changes into your working branch, first commit your current work, then run:

```bash
git fetch origin
git merge origin/main
```

If conflicts appear:

1. Open the affected files and decide which changes to keep with your teammate.
2. Remove the conflict markers and save the files.
3. Run the programs to check the combined changes.
4. Stage the resolved files, commit, and push:

   ```bash
   git add <resolved-file>
   git commit -m "Resolve merge conflicts with main"
   git push
   ```

## Learning Objectives

- Write and run basic Python programs.
- Track changes using Git.
- Create and manage branches.
- Submit and review pull requests.
- Resolve merge conflicts.
- Collaborate with teammates and document project work.
s