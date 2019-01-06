# What is Git?

![Git Defined](img/define-git.png)

Git is a version control system. Version control systems track the set of changes applied to files, and allow for
users to switch between versions of these files. It also allows for the distribution of files, which
enables teams to work in sync with each other.

## Who uses Git?

Tons of individuals and organizations use Git.

- Amazon, Microsoft, Facebook, Netflix, Linux, Android, Eclipse, Starbucks, Google...
- Over 31 million users on GitHub (note: Git != GitHub)
- Your classmates!

## Why use Git?

As with any version control system, Git offers some nice features:

- Lets you keep your files in sync.

  - Works across workstations, like your laptop and desktop
  - Works across teams, each member can get the latest changes

- Backs up your source code.

  Because your files can be backed up to GitHub or some other host, you have much less risk of losing
  your files due to hardware failures.

- Enables for distributed collaboration.

  Multiple team members can work remotely on the same set of files, no matter their location.

- Manage complex workflows.

  Git enables teams of any size to contribute to projects, all at the same time.
  This is why so many organizations use Git to develop large-scale open source projects,
  like the Linux Kernel, Firefox, and many more.

- Tracks your revision history.

  You can rollback changes to any state at any time.
  This is great for working on features or breaking changes, while
  maintaining a stable copy of the project at the same time.

## What isn't Git?

It's important to make a few distinctions when describing the features that Git provides.

### Git is not GitHub/GitLab/BitBucket

Git is a version control tool. Git can connect to a remote server to sync files. Git
does not need internet access to function, and can run independently of the internet.

GitHub is a website that host repositories. GitHub integrates with Git to show information
about Git repositories, and provides it's own set of tools on top of Git to enhance workflows.
GitHub has features like Issues, Pull Requests, and Continuous Integration.

Common alternatives to GitHub are GitLab, BitBucket, etc. Git can work with these interchangeably just fine.
The differences between these are not described here.

### Git is not Google Drive/Dropbox/etc.

While Git does allow for real-time collaboration on projects, it does not allow for simultaneous changes by multiple
authors, like you would see in Google Docs.
Instead, batches of changes are made by individual authors which then are merged into the overall codebase.

That being said, Git is still an industry-standard tool for collaborative software development.
There are some tools that can allow for simultaneous Google Docs-like file editing, but we will not cover these here.