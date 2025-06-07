
# Git
- git is version control systme (vms)
-  Nearly every developer in the world uses it to manage their code
- Keep a history of their code changes
- Revert mistakes made in their code
- Collaborate with other developers
- Make backups of their code 

# Command Syntax
- `command <required> [optional]`

# Quick Config
- git config --get user.name
- git config --get user.email

# Config
- git init

# Status

- `git status`
- untracked: Not being tracked by Git
- staged: Marked for inclusion in the next commit
- committed: Saved to the repository's history

# Git Log

- The git log command shows a history of the commits in a repository. This is what makes Git a version control system. You can see:

- Who made a commit
- When the commit was made
- What was changed
- `git log`
- `git --no-pager log -n 3` show recent 3 log

![image](https://github.com/user-attachments/assets/f15a9c51-a33c-4186-808c-bcb155abc3a3)


# Cat File
- git cat-file is a low-level Git command used to inspect Git objects (like commits, trees, blobs, or tags) directly from the Git object database.
-  Common Options:
- Option	Description
- -t	Show the type of the object (commit, blob, tree, tag).
- -s	Show the size of the object in bytes.
- -p	Pretty-print the content of the object.

![image](https://github.com/user-attachments/assets/5d04f734-370e-4261-82d4-dbecfce61ebf)

# What Is a Branch?

- A Git branch allows you to keep track of different changes separately.
- Check your current branch:
- `git branch`

# How to Rename a Branch
- `git branch -m oldname newname`

# New Branch
- git branch my_new_branch
- git switch -c my_new_branch

# What is git rebase?

- git rebase is a Git command used to move or combine a sequence of commits to a new base commit. It's commonly used to:

# Git Reset Soft

- The git reset command can be used to undo the last commit(s) or any changes in the index (staged but not committed changes) and the worktree (unstaged and not committed changes).
- `git reset --soft COMMITHASH`
- 





# 📚 Common Branch Type Prefixes

| Prefix                | Purpose                                      |
| --------------------- | -------------------------------------------- |
| `feature/` or `feat/` | New features or enhancements                 |
| `bugfix/` or `fix/`   | Bug fixes                                    |
| `hotfix/`             | Critical fixes to production                 |
| `release/`            | Prepares for a production release            |
| `test/`               | Experimental or testing branches             |
| `chore/`              | Maintenance or minor changes                 |
| `refactor/`           | Code improvements with no change in behavior |
| `docs/`               | Documentation changes                        |
| `ci/` or `devops/`    | CI/CD or infrastructure changes              |


# 📌 Examples

`feature/user-login`
`feat/add-search-bar`
`bugfix/fix-crash-on-startup`
`hotfix/memory-leak-production`
`release/v2.3.0`
`docs/update-readme`
`chore/cleanup-unused-code`
`refactor/auth-service`
`ci/add-github-actions`


## 📘 Resources

- [Learn Git Course on Boot.dev part 1](https://www.boot.dev/courses/learn-git)


