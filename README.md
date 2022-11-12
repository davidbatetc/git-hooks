# Useful git hooks
To add these hooks to your git repository, remove the folder `hooks` inside your `.git` folder and clone this repository inside `.git`. In Unix-like systems:
```sh
$ rm -r .git/hooks
$ git clone <link-to-repository> .git/hooks
```

Alternatively, clone this repository somewhere else and create a symbolic link called `hooks` inside the `.git` repository. In Unix-like systems:
```sh
$ git clone <link-to-repository> <chosen-path>
$ ln -s <chosen-path> .git/hooks
```
If you want to use a relative `<chosen-path>` make sure that it is relative to the `.git` folder when creating the symbolic link. The following command should not produce any output:
```sh
$ test -e .git/hooks || echo "Broken symbolic link"
```
