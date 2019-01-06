# Git Glossary and Reference

This is a reference to git vocabulary and a brief commands reference.

## Repository

A repository is a set of files. Repositories can have a set of branches, each with their own set of commits.
Generally the default branch is called `master`, which contains the initial commit.

## Branch

A set of commits that are related to each other. The default branch is typically called `master`.
When new branches are created from another branch, their commits will always refer back to commits in that original branch.
Branches are great for working on small and incremental changes, while ensuring that the `master` branch isn't broken.
When work on a specific branch is done, it can be merged back into another branch. During a merge, all of the commits that
have been added are copied to the destination branch.

## Commit

A set of changes to files, that have been "committed" into the repository.
Commits always have these properties:

- A commit message, which is a description of the changes made
- A set of additions and deletions to files in the repository
- A commit hash, used for identification
- A commit author
- A commit timestamp