# Create-github-action-boilerplate

Creates a boilerplate github action ready to be published - based off [Githubs official guide ](https://help.github.com/en/actions/automating-your-workflow-with-github-actions/creating-a-javascript-action#commit-and-push-your-action-to-github)

## Quick overview

```
npx run create-github-action my-action
cd my-action
```

From there add it github by

```
git init
git add .
git commit -m init
git push --set-upstream origin master
```

From there go to your repository on github and click "Publish this action to marketplace" following
[this guide](https://help.github.com/en/actions/automating-your-workflow-with-github-actions/publishing-actions-in-github-marketplace#publishing-an-action).

### Use in workflow

```- name: Hello world
      uses: actions/my-action@v1
      with:
        who-to-greet: 'Mona the Octocat'
```
