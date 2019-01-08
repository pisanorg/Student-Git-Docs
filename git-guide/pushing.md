# Syncing your local repository to GitHub

Git can work completely offline, but it's likely that you'll want to sync your repo with a service like GitHub.
You'll need to do this if your class is using GitHub Classroom.

Unlike services like Dropbox or Google Drive, changes are not synced automatically. Instead, you'll need to tell Git
to do this manually. A `push` is when you upload changes to a server, and a `pull` is when you download changes from a server.
Git will only push and pull commits, so uncommitted files will not be synced.

Typically, it's best that you `pull` before you start any work, and right before you `push` new changes. This ensures
that you have the latest version of the repository.

## Uploading your changes

If you `git clone`d the repository, Git will automatically set the remote (server) URLs for you.


## Pulling changes from GitHub

To pull any changes from the GitHub branch to your local repository simply run `git pull`.

**NOTE** You might run into merge conflicts if you committed changes to your local repository before it's fully synced with the GitHub repository. We will not be covering how to deal with merge conflicts in this tutorial. 

[Learn more about how to resolve merge conflicts here](https://help.github.com/articles/resolving-a-merge-conflict-using-the-command-line/).