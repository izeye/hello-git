# Hello, Git!

## Commands

### git format-patch

* Create a patch:

```bash
git format-patch -n HEAD^
```

* Apply the patch:

```bash
git am 0001-Add-README.md.patch
```

### git bundle

#### Initial sync

* Create a Git bundle:

```bash
git bundle create file.bundle master
```

* Clone from the Git bundle:

```bash
git clone -b master file.bundle hello-git
```

#### Subsequent syncs

* Create a Git bundle for changes 10 days ago:

```bash
git bundle create file.bundle --since=10.days master
```

* Pull the changes from the Git bundle:

```bash
git pull
```
