# github-commands
useful github or git commands that are not common enough to memorize

* Update git authorship (only use on repositories with no other users!, useful if work computer puts incorrect author on commits)

git filter-branch -f --env-filter "GIT_AUTHOR_NAME='mcmenemy'; GIT_AUTHOR_EMAIL='mr_mcmenemy@yahoo.com'; GIT_COMMITTER_NAME='mcmenemy'; GIT_COMMITTER_EMAIL='mr_mcmenemy@yahoo.com';" HEAD

* Push a remote which is not upstream of current branch

git push --set-upstream <origin> master

* Remove a file from git repository but not local (like if you accidently pushed node modules)
git rm -r --cached node_modules
git commit -m 'remove the now ignored directory node_modules'  # make sure you added folder to .gitignore
git push

