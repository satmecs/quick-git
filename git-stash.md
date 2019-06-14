## GIT STASH

This command is simple. The workflow would be as follows.

1. Make sure branch is clean (check with git status)
2. Make some changes to the project.
3. Run `git stash save 'MSG'` (working directry will be clean again)
4. View stashed tags with `git stash list`
5. Switch to any stash using `git stash apply stash{0}` 
6. Make some more changes again and push a new stash if you are again not done.
7. This new stash will get tagged as `stash{0}` and previous will get pushed down the stack.
8. If you popped any stash and wanna get back to clean state run `git checkout -- .`