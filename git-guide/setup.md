# First-Time Git Setup

This guide contains information about first-time setup with Git.

## Step 0. Install Git

[If you haven't installed Git yet, please refer to this document for those instructions.](../installing-git.md)

## Step 1. Make a GitHub account

[If you haven't made a GitHub account yet, please refer this documentation for those instructions.](../make-a-github-account.md)

## Step 2. Verify Installation

After installing Git, verify that your installation works as expected.

Open a new terminal window. On Windows, this is Command Prompt, and on Linux or Mac you can use terminal.

Run the following command:

```console
git --version
```

You should see text similar to `git version 2.X.X`.

If you don't see this text, [please refer to the troubleshooting steps in the installation guide.](../installing-git.md)


## Step 3. Configuration

Before you can get started with Git, you'll have to configure a few things first.

Run the following commands, but with your name and email. Make sure to use the same email that you used for your GitHub account.

```console
git config --global user.name "Bobby Tables"
git config --global user.email "BobbyTables@uw.edu"
```
