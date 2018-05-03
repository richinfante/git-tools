# SSH Shortcuts for git

For self-hosted git, I follow the convention that all bare repos are in the
user's $HOME/git directory. This way, it's uniform across all my systems
and allows me to easily backup and retrive data from them.

These scripts were made with this in mind. Place them in your path, and
you'll be able to do the following:


## REMOTE-LS
Usage: `git remote-ls [hostname]`
```bash
# List repos in the git/ directory.
~# git remote-ls my-server
app-repo.git/
thing.git/
notes.git/
website.git/
```

## REMOTE-CLONE
Usage: `git remote-clone [hostname] [reponame]`
```bash
git remote-clone my-server website
cloning into "website"...
```

## REMOTE-CREATE
Usage: `git remote-create [hostname] [reponame]`

Create a bare repo on the remote. Repos are created as `[reponame].git`

```bash
git remote-create my-server secret-project
```


