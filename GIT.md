# My Git CHEATS


## En Vrac
```sh
$ git update-index --chmod=+x execute.sh
$ git ls-files --stage
$ git add --all
```
## Git Flow Without Cammand

```sh
$ git checkout -b feature/toto develop
$ git checkout develop
$ git merge --no-ff feature/toto
$ git branch -d feature/toto
$ git push origin develop
```

## Git Flow
```sh
$ apt-get install git-flow
```
### Initialize
```sh
$ git flow init
```
### Start a new feature
```sh
$ git flow feature start MYFEATURE
```
### Finish up a feature
```sh
$ git flow feature finish MYFEATURE
```
### Publish a feature
```sh
$ git flow feature publish MYFEATURE
```
### Getting a published feature
```sh
$ git flow feature pull origin MYFEATURE
$ git flow feature track MYFEATURE
```
### Start a release
```sh
$ git flow release start RELEASE [BASE]
$ git flow release publish RELEASE
$ git flow release track RELEASE
```
### Finish up a release
```sh
$ git flow release finish RELEASE
$ git push --tags
```
### git flow hotfix start
```sh
$ git flow hotfix start VERSION [BASENAME]
$ git flow hotfix finish VERSION
```