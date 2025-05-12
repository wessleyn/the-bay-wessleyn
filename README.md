# Shipwreck : The Bay

This is a superrepo that links to all my 4 projects for the bay program using Git submodules.

## What are the folders

Each folder is a Git submodule that links to the repo or the project that I have done for the bay program.

The folders are named after the project or the repo that they link to.

## How to use this repo

1. Clone the repo with submodules

   ```bash
   # Clone the repo including all submodules (recommended)
   git clone --recurse-submodules https://github.com/wessleyn/the-bay-wessleyn.git
   cd the-bay-wessleyn

   # Or clone normally and then initialize submodules separately
   git clone https://github.com/wessleyn/the-bay-wessleyn.git
   cd the-bay-wessleyn
   git submodule init
   git submodule update
   ```

2. Go to the folder that you want to use

   ```bash
   cd project-folder-name
   ```

3. Follow the instructions in the README.md file in that folder

   ```bash
   cat README.md  # View the README file
   # Or open with your text editor
   ```

4. If you have any questions, feel free to ask me on discord or open an issue in the repo

   ```bash
   # To open an issue on GitHub:
   # Go to https://github.com/wessleyn/the-bay-wessleyn/issues/new
   ```

5. If you want to contribute to the repo, feel free to open a pull request

   ```bash
   # Fork the repo on GitHub first
   git checkout -b your-feature-branch
   # Make your changes
   git add .
   git commit -m "Description of your changes"
   git push origin your-feature-branch
   # Then create a pull request on GitHub
   ```

6. If you want to add a new project, feel free to open a pull request
   ```bash
   # To add a project as a submodule
   git submodule add https://github.com/wessleyn/your-project.git new-project-name
   git commit -m "Add new project: new-project-name"
   git push origin main
   ```

## Working with submodules

```bash
# Update all submodules to latest remote version
git submodule update --remote

# Pull changes in all submodules
git pull --recurse-submodules

# Check status of all submodules
git submodule status

# Execute a command in each submodule
git submodule foreach 'git status'
```
