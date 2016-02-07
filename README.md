# github-commands
useful github or git commands that are not common enough to memorize

* Update git authorship (only use on repositories with no other users!, useful if work computer puts incorrect author on commits)

git filter-branch -f --env-filter "GIT_AUTHOR_NAME='mcmenemy'; GIT_AUTHOR_EMAIL='mr_mcmenemy@yahoo.com'; GIT_COMMITTER_NAME='mcmenemy'; GIT_COMMITTER_EMAIL='mr_mcmenemy@yahoo.com';" HEAD
