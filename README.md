```
git submodule init
git submodule sync
```

```
git submodule add https://path-to-readonly/repo1.git @hard-apps/repo1
git submodule add https://path-to-readonly/repo2.git @hard-apps/repo2
```

add repo2 to repo1:

```
cd @hard-apps/repo1
npm i @hard-apps/repo2
```

### Adding new submodule app

```
mkdir @hard-apps/new-app
cd @hard-apps/new-app
git init
git remote add origin <origin>
cp ../../.gitignore .
```

## Add tsc to every package.json

```
"script": {
	"tsc": "tsc"
}
```
