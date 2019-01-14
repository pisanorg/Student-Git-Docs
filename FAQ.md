# Frequently Asked Questions (FAQ)

- [Repository Not Found While Cloning with Valid URLs](#repo-not-found)

## Repository Not Found While Cloning with Valid URLs<a name="repo-not-found" />

If you are having trouble cloning your repository after you have accepted the
GitHub Classroom assignment and see this error...

```
$ git clone https://github.com/<CLASSROOM>/<ASSIGNMENT>-<USERNAME>.git
Cloning into '<ASSIGNMENT>-<USERNAME>'...
remote: Repository not found.
fatal: repository 'https://github.com/<CLASSROOM>/<ASSIGNMENT>-<USERNAME>.git/' not found
```

...then please delete any directory that may have been created and retry with
your username in the URL:

```
$ git clone https://<USERNAME>@github.com/<CLASSROOM>/<ASSIGNMENT>-<USERNAME>.git
```
