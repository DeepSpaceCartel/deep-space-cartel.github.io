# Deep Space Cartel

* https://deep-space-cartel.github.io/
* https://deepspacecartel.com/

## `mkdocs`

* https://www.mkdocs.org/
* https://squidfunk.github.io/mkdocs-material/

### Development

```
mkdocs serve
```

### Deployment

```
mkdocs gh-deploy
```

### TODO

- [x] Switch to VSCode native container.
- [ ] Enable mkdocs container feature.
- [ ] Create [feature-starter](https://github.com/devcontainers/feature-starter) to replicate [`squidfunk/mkdocs-material:8.5.11`](https://github.com/squidfunk/mkdocs-material/blob/master/Dockerfile) image.
- [x] Enable colors support for git diff.
- [ ] Install and configure pre-commit feature.
- [ ] Configure and document commit signing.

### Known Problems

#### Missing gpg keys

```
$ git commit
...
error: gpg failed to sign the data
```

```
alexa@DESKTOP-TNINHI3 MINGW64 ~
$ cat ~/.gitconfig
[filter "lfs"]
        clean = git-lfs clean -- %f
        smudge = git-lfs smudge -- %f
        process = git-lfs filter-process
        required = true
[user]
        name = Alexander Ilyin
        email = alexander@ilyin.eu
        signingkey = CA6878224D0AE67D
[commit]
        gpgsign = true
```

```
git commit --no-gpg-sign ...
```
