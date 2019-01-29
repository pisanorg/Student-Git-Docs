# Frequently Asked Questions (FAQ)

- [Repository Not Found While Cloning with Valid URLs](#repo-not-found)
- [CLion: "error while loading shared libraries: ?: cannot open shared object file: No such file or directory"](#msys)
- [bad interpreter: no such file or directory](#line-endings)

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

## Error while loading shared libraries ... <a name="msys">

This issue can occur when performing a Git Push in clion.

You may see an error similar to this:

```
C:/msys64/usr/lib/git-core/git-remote-https.exe: error while loading shared libraries: ?: cannot open shared object file: No such file or directory
```

[A solution can be found here: https://stackoverflow.com/questions/35191375/msys2-git-on-windows-errors-looking-for-shared-object-file/35236385#35236385](https://stackoverflow.com/questions/35191375/msys2-git-on-windows-errors-looking-for-shared-object-file/35236385#35236385)

This is fixed by changing the path to the Git executable in CLion.

## Resolving Line Endings Issues on Linux<a name="line-endings" />

When a `.sh` script file has been copied to a Linux file system
from Windows, running this script may produce this error:

```
bad interpeter: no such file or directory
```

This issue can happen because of the line endings of the file.
By default Windows uses `CRLF` line endings, while Mac/Linux use `LF`.
Windows `CRLF` line endings are not compatible with linux `.sh` bash script files.

There are two solutions for this issue:
1. Convert the line endings of the file using the `dos2unix` tool.
    ```console
    dos2unix myscript.sh
    ```
2. Instead of copying files from Windows to Linux, use `git` instead to sync them. Unless file ending settings are overwritten, `git` should handle these for you.