# Syncing your local repository to GitHub

Git can work completely offline, but it's likely that you'll want to sync your repo with a service like GitHub.
You'll need to do this if your class is using GitHub Classroom.

Unlike services like Dropbox or Google Drive, changes are not synced automatically. Instead, you'll need to tell Git
to do this manually. A `push` is when you upload changes to a server, and a `pull` is when you download changes from a server.
Git will only push and pull commits, so uncommitted files will not be synced.

Typically, it's best that you `pull` before you start any work, and right before you `push` new changes. This ensures
that you have the latest version of the repository.

## Uploading your changes

If you run `git status` and see a message like this:

```
On branch master
Your branch is ahead of 'origin/master' by 1 commit.
  (use "git push" to publish your local commits)
nothing to commit, working directory clean
```

It means that your local `master` branch has a new commit that does not exist on `origin` (origin is the name given to your remote server, in this case GitHub).
You can upload this change to the remote server by typing `git push`. You'll see a prompt to enter your GitHub credentials. The login prompt will not show
any indication while you are typing in your password, so just press enter when you are finished.

You should see output similar to this:

```
$ git push
Counting objects: 6, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 1.85 KiB | 0 bytes/s, done.
Total 6 (delta 4), reused 0 (delta 0)
remote: Resolving deltas: 100% (4/4), completed with 4 local objects.
To git@github.com:pisanorg/Student-Git-Docs.git
   754de7f..5629551  master -> master
```

You can verify that these changes have been uploaded without errors by viewing your repo on GitHub.
In this case, I can see that my latest commit was created `5 minutes ago`, so the push worked without errors.
Pushing code does not alter the timestamps for commits, time is stored when commits are made and is not modified.
While I pushed less than a minute ago, the commit was authored 5 minutes ago.

![pushed commit on github](img/pushed-commit.PNG)

### Uploading a new branch

If you tried `git push` on a new branch, or only saw the output `Everything up-to-date`, even though you've made changes, you'll need to try a different command.

It's possible that your branch does not exist on GitHub. By default, new branches are not created automatically.
To create this new branch, use `git status` to determine your current branch, then run the following:

```console
$ git status
On branch newbranch

$ git push -u origin newbranch
Total 0 (delta 0), reused 0 (delta 0)
remote:
remote: Create a pull request for 'newbranch' on GitHub by visiting:
remote:      https://github.com/pisanorg/Student-Git-Docs/pull/new/newbranch
remote:
To git@github.com:pisanorg/Student-Git-Docs.git
 * [new branch]      newbranch -> newbranch
Branch newbranch set up to track remote branch newbranch from origin.
```

This will create this new branch on GitHub. You'll only need to do this once, and `git push` should start to work as expected.

## Pulling changes from GitHub

To pull any changes from the GitHub branch to your local repository simply run `git pull`.

**NOTE** You might run into merge conflicts if you committed changes to your local repository before it's fully synced with the GitHub repository. We will not be covering how to deal with merge conflicts in this tutorial. 

[Learn more about how to resolve merge conflicts here](https://help.github.com/articles/resolving-a-merge-conflict-using-the-command-line/).

### Git Pull Vs Git Fetch

[This is explained well by this StackOverflow post.](https://stackoverflow.com/questions/292357/what-is-the-difference-between-git-pull-and-git-fetch)

`git pull` executes two actions, it first downloads the latest information from the server, then applies these changes to your local repository.
If you only want to download the latest information from the server without applying changes, then you can use `git fetch`.