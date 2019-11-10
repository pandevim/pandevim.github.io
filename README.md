```bash
$ mkdir GITHUB-USERNAME.github.io
$ hub init && hub create -d "my happy place"
$ hub checkout dev
$ curl -o .gitignore https://raw.githubusercontent.com/github/gitignore/master/Node.gitignore
$ curl -o .gitattributes https://raw.githubusercontent.com/alexkaratarakis/gitattributes/master/Web.gitattributes
$ hub push --set-upstream origin dev
$ hub checkout --orphan master && hub rm -rf .
$ hub commit --allow-empty -m "Init Build Branch"
$ hub push --set-upstream origin master
$ hub checkout dev && echo "\n\nbuild/" >> .gitignore
$ hub worktree add build master
$ hub push
```