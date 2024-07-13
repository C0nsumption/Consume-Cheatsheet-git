# Consume-Cheatsheet-git 🤓

Yo, check it out! This is your go-to cheatsheet for Git commands, cool tricks, and workflow stuff.

<details>
<summary>WHAT'S THE DEAL WITH GIT? 🤔</summary>

Listen up, here's the 411 on Git: A repo (that's short for repository) 🗃️ is basically just a fancy folder for your project. It keeps tabs on all your files and any changes you make to 'em.

Wanna try something new without messing up your masterpiece? That's where branches come in 🍂. It's like making a copy you can mess around with, no strings attached.

Pro tip: Make a main branch, a dev branch, and feature branches for any cool new stuff you wanna add! Merge your features into dev, make sure everything's cool, then merge dev into main. Easy peasy.

</details>

<details>
<summary>WHAT'S THE DEAL WITH GITHUB AND BITBUCKET? ☁️</summary>

GitHub and Bitbucket? They're just websites where you can stash your repos. But don't get it twisted, they ain't Git itself 😎. They're just making it stupid easy to keep your stuff in the cloud and work with your coding buddies. 👥

So here's the deal: Git's watching your project files, branches let you do your thing without stepping on anyone's toes. GitHub and Bitbucket? They're just giving your stuff a home online. Got it? Sweet. 👌

</details>

<details>
<summary>Git Commands</summary>

* `git init` - Kick off a local repo
* `git clone` - Snag a copy of a repo
* `git add` - Toss files into staging
* `git commit` - Lock in your changes locally
* `git push` - Shove your changes up to the remote
* `git pull` - Grab the latest changes
* `git status` - See what's up with your files
* `git log` - Peep your commit history
* `git branch` - Handle your branches
* `git checkout` - Hop between branches
* `git merge` - Smoosh branches together
* `git remote` - Deal with remote repos
* `git fetch` - Snatch the latest objects
* `git reset` - Hop back to a commit
* `git revert` - Undo commits
* `git tag` - Slap labels on stuff
* `git stash` - Hide your changes for later
* `git clean` - Kick out untracked files
* `git config` - Tweak your settings
* `git diff` - Spot the differences in files

</details>

## Common Patterns

### How do I create a repo? 🤔

```bash
git init 
git add .
git commit -m "initial: first blood"
git branch -M main  # This renames the current branch to 'main'
```

### How do I make a branch on my repo? 🤔

```bash
git checkout -b feature-branch
git add .
git commit -m "feat: started work on awesome new feature"
```

### 🥺 Damnit, I already made changes but forgot to make a branch. How do I make a branch without losing my changes? 🤨

```bash
git stash 
git checkout -b feature-branch
git stash pop
git add .
git commit -m "feat: started work on awesome new feature"
```

### 🙈 I messed up my last commit message. How do I fix it?

```bash
git commit --amend -m "feat: what I actually meant to say"
```

### 🔀 How do I merge main into my feature branch to stay up-to-date?

```bash
git checkout feature-branch
git merge main
# Resolve any conflicts if they occur
git add .
git commit -m "merge: main into feature-branch"
```

### How do I get the most recent changes to their project or repo? 🙄

```bash
git fetch  # Grab the latest changes
git pull <branch>  # Yank down the latest branch
git add .  # Stage all your changed files
git commit -m "<message>"  # Lock in those changes
git push  # Launch your commits to the remote
```