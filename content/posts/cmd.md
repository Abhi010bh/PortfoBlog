+++
title = 'Development helps'
date = 2023-12-14T22:01:26+05:30
draft = false
+++

## NPM/Yarn Commands

### Installing Dependencies
{{< highlight bash >}}
- `npm install <package>`: Installs a package.
- `npm install`: Installs all dependencies listed in `package.json`.
- `yarn add <package>`: Adds a package using Yarn.
{{< /highlight >}}

### Running Scripts
{{< highlight bash >}}
- `npm start`: Runs the script defined as "start" in `package.json`.
- `npm run <script-name>`: Executes a custom script defined in `package.json`.
- `yarn start`: Runs the start script using Yarn.
{{< /highlight >}}

### Managing Dependencies
{{< highlight bash >}}
- `npm uninstall <package>`: Uninstalls a package.
- `npm update <package>`: Updates a package.
- `yarn remove <package>`: Removes a package using Yarn.
- `yarn upgrade <package>`: Upgrades a package using Yarn.
{{< /highlight >}}

## Git Commands

### Git Initialization
{{< highlight bash >}}
- `git init`: Initializes a new Git repository.
{{< /highlight >}}

### Staging and Committing
{{< highlight bash >}}
- `git add .`: Adds all changes to the staging area.
- `git commit -m "commit message"`: Commits changes with a message.
{{< /highlight >}}

### Branching and Merging
{{< highlight bash >}}
- `git branch`: Lists branches.
- `git checkout -b <branch-name>`: Creates and switches to a new branch.
- `git merge <branch-name>`: Merges a branch into the current branch.
- `git pull origin <branch-name>`: Pulls changes from a remote branch.
- `git push origin <branch-name>`: Pushes changes to a remote branch.
{{< /highlight >}}

## Running Node.js

### Starting Node Server
{{< highlight bash >}}
- `node server.js`: Starts the Node.js server.
{{< /highlight >}}

### Running Scripts
{{< highlight bash >}}
- `nodemon <script.js>`: Automatically restarts the Node.js server on file changes (if you've installed Nodemon).
{{< /highlight >}}

## Miscellaneous

### Terminal Navigation
{{< highlight bash >}}
- `cd <directory>`: Changes the current directory.
- `ls` (Unix) / `dir` (Windows): Lists files and directories.
{{< /highlight >}}

### File Operations
{{< highlight bash >}}
- `touch <file-name>`: Creates a new file (Unix).
- `echo > <file-name>`: Creates a new file (Windows).
- `rm <file-name>`: Removes a file (Unix).
- `del <file-name>`: Deletes a file (Windows).
{{< /highlight >}}
