This exercise will guide you to the basic git workflow of contributing your code to existing projects.

# Fork

**Fork repo** by clicking on the fork button on the top of this page.
This will copy my repo and 'paste' it under your Github account.

# Clone

**Clone your forked repository** to your computer. Go to your GitHub account, open the forked repository, click on the green code button and then click the _copy to clipboard_ icon.

Open a terminal and run the following git command:

```
git clone "url you just copied"
```

# Branch

**Create a branch** - Change to the repository directory on your computer (if you are not already there):

```
cd git-branch-pr-workflow
```

Now create a branch using the `git checkout` command:

```
git checkout -b your-new-branch-name
```

For example, you can create a branch using your initials:

```
git checkout -b add-AV
```

(The name of the branch does not need to have the word _add_ in it, but it's a reasonable thing to include because the purpose of this branch is to add your name to a list.)

# Edits

**Make changes** - Open contributors.md; add your initials and github link using markdown format such as: `[AV](http://github.com/avcoder)`

If you go to the project directory and execute the command `git status`, you'll see there are changes.

# Add

**Add those changes** to the branch you just created using the `git add` command:

```
git add contributors.md
```

# Commit

**Commit those changes** using the `git commit` command:

```
git commit -m "Add <your-initials> to Contributors list"
```

replacing `<your-initials>` with your initials.

# Push branch

**Push changes** to GitHub

Push your changes using the command `git push`:

```
git push origin <add-your-branch-name>
```

replacing `<add-your-branch-name>` with the name of the branch you created earlier.

# Pull Request (PR)

**Compare & Pull request** - Submit your changes for review

If you go to your repository on GitHub, you'll see a `Compare & pull request` button. Click on that button.

Now submit the pull request.

Soon I'll be merging all your changes into the master branch of my repo.

Congrats! You just completed the standard _fork -> clone -> edit -> pull request_ workflow that you'll encounter often.
