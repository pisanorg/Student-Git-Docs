# Branching and Merging

## Checking out a new branch

To create a new branch from your current branch, run the following command:

```
  git checkout -b [NEW_BRANCH_NAME_GOES_HERE]
```

You can verify that you have created and switched to the new branch by running `git status`.

## Switch to an existing branch

To switch to an existing branch that's different from your current branch, run the following command:

```
  git checkout BRANCH_NAME_TO_SWITCH_TO_GOES_HERE
```

**NOTE** If you have uncommitted changes, those changes will be carried over into the branch you switch to.

## Pushing the current branch to GitHub

After setting the remote URL, you can push your current branch (if you have write-access to the GitHub repository you're hoping to push to) to GitHub by running:

```
  git push origin -u BRANCH_NAME_GOES_HERE
```

You can verify if this command worked by navigating to your repository's webpage. You should see your branch listed in the branch list.

## Merging branches

In order to merge branches simply run the following command:

```
  git merge BRANCH_NAME_TO_MERGE_WITH_GOES_HERE
```

This will merge the branch specified into the current branch.

**NOTE** You might run into merge conflicts if two different commits from the base and merging branch change the same line in the same file. We will not be covering how to deal with merge conflicts in this tutorial.