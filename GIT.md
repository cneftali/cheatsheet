# My Git CHEATS


## En Vrac

$ git update-index --chmod=+x execute.sh
$ git ls-files --stage
$ git add --all

## Git Flow

$ git checkout -b feature/toto develop
$ git checkout develop
$ git merge --no-ff feature/toto
$ git branch -d feature/toto
$ git push origin develop

$ apt-get install git-flow

### Initialize

$ git flow init

### Start a new feature

$ git flow feature start MYFEATURE

### Finish up a feature

$ git flow feature finish MYFEATURE

### Publish a feature

$ git flow feature publish MYFEATURE

### Getting a published feature

$ git flow feature pull origin MYFEATURE
$ git flow feature track MYFEATURE

### Start a release

$ git flow release start RELEASE [BASE]
$ git flow release publish RELEASE
$ git flow release track RELEASE

### Finish up a release

$ git flow release finish RELEASE
$ git push --tags

### git flow hotfix start

$ git flow hotfix start VERSION [BASENAME]
$ git flow hotfix finish VERSION