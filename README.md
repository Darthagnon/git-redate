# git-redate
### Made by [Potato Labs](http://taterlabs.com)

Change the dates of several git commits with a single command.

![Demonstration of git redate](/yE4cQ.gif)

# Installation

For homebrew users, you need to run `brew tap PotatoLabs/homebrew-git-redate` and then `brew install git-redate`.

If you're not using homebrew, you can clone this repo and move the `git-redate` file into any folders in your $PATH. Restart your terminal afterwards and you're good to go!

For window's users, you may paste the file into `${INSTALLATION_PATH}\mingw64\libexec\git-core`. Assuming you used the default settings the installation path will be `C:\Program Files\Git`.

# Usage

Simply run: `git redate --commits [[number of commits to view]]`.  You'll have to force push in order for your commit history to be rewritten.

To be able to edit all the commits at once add the --all option: `git redate --all`

**Make sure to run this on a clean working directory otherwise it won't work.**

The `--commits` (a.k.a. `-c`) argument is optional, and defaults to 5 if not provided.

## See also

> You can do an interactive rebase and choose edit for the commit whose date you would like to alter. When the rebase process stops for amending the commit you type in for instance: 
> `git commit --amend --date="Wed Feb 16 14:00 2011 +0100" --no-edit` 
> P.S. `--date=now` will use the current time.
> 
> Afterward, you continue your interactive rebase.
> 
> To change the commit date instead of the author date:
> `GIT_COMMITTER_DATE="Wed Feb 16 14:00 2011 +0100" git commit --amend --no-edit`
> 
> The lines above set an environment variable GIT_COMMITTER_DATE which is used in amending commit.
> 
> Everything is tested in Git Bash.

- [How can one change the timestamp of an old commit in Git? on StackOverflow](https://stackoverflow.com/questions/454734/how-can-one-change-the-timestamp-of-an-old-commit-in-git)
