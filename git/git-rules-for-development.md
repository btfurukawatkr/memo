## git setting
 * name
 * email

## git command
 * git clone [url]
  - create a repository to your local work-space
 * git checkout [branch-name]
  - swith to working-branch
 * git checkout -b [branch-name]
  - create a new branch to your local repository
 * git pull
  - update your working-branch
 * git status
  - check your local-repository's status
 * git add [file]
  - add updated file
 * git commit -m "[message]"
  - commit added files
  - issue number must be typed at the end of message as #[issue-number]
 * git push [remote name] [branch-name]
  - send commit info to remote server
 * git branch -D [branch-name]
  - delete branch from your local repository

## merging same fix to a diffrent branch
 * git cherry-pick -x [commit-hash-number]

## incase there was a conflict when you tried to push
 * git rebase [original-branch-name]
  - update working branch to [original-branch-name], and re-commit your already-committed files
 * git push -f [remote name] [branch-name]
  - -f option will force the remote branch tobe replaced with the pushing branch

# undo changes in your local repository which is not committed yet
 * git checkout .

# undo changes in your local repository which has been committed
 * git revert -m 1 [commit-hash-number]

