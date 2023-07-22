# cheatsheet-git 🤓
A 'cheatsheet' for Git commands, practices, and workflow.

## WHAT IS GIT? 🤔
So here's a quick and dirty briefing on Git: A repository aka repo 🗃️ is like a folder for your project. It tracks all files within it and any changes made to 'em.

You can branch off 🍂 the main repo (like making a copy that you can edit without damaging the original) to try new things without messing up the original. Branches let you work on features independently then merge 'em back to the main branch when ready.

If you know whats good for ya, you'll make a main branch, a dev branch, and feature branches for any new features you want to add! Then we merge our features into the dev branch. If everything checks out, we merge our dev branch into our main.

## WHAT ABOUT GITHUB AND BITBUCKET?! ☁️
GitHub and Bitbucket are popular websites for hosting repos. But don't get it twisted, they ain't Git 😎 itself. They just make it easy to store your repos in the cloud and collaborate with other developers. 👥

So: Git tracks your project files and branches help you work without trippin' over your team. GitHub and Bitbucket host your stuff online. Capisce? 👌

## Git Commands

- `git init` - Initialize local repository
- `git clone` - Clone repository
- `git add` - Add files to staging  
- `git commit` - Commit changes locally
- `git push` - Push changes to remote
- `git pull` - Pull latest changes
- `git status` - List file status
- `git log` - Show commit history
- `git branch` - Manage branches
- `git checkout` - Switch branches
- `git merge` - Merge branch
- `git remote` - Manage remote repos
- `git fetch` - Fetch latest objects
- `git reset` - Reset to commit
- `git revert` - Revert commits
- `git tag` - Manage tags  
- `git stash` - Stash changes
- `git clean` - Remove untracked files
- `git config` - Get/set options
- `git diff` - Show file differences

## Common Workflow

- `git fetch` - Fetch latest changes
- `git pull <branch>` - Pull latest branch
- `git add .` - Stage all changed files 
- `git commit -m "<message>"` - Commit changes
- `git push` - Push commits to remote
