# Installation
1. Place these scripts in a persistent location.
2. Add the location to `PATH`.

# Usage
```
$ git browse
$ git lazy
$ git produce
```

## Git Browse
* Opens the repository in your default web browser. Note: only GitHub, GitLab, and BitBucket remotes are supported.

> The environment variable `BROWSER` must be set.

## Git Lazy
* Commits and pushes all modified + untracked files.

## Git Produce
* Creates (or updates) a production branch from master. Then pushes the branch.
	* See [GitLab Flow](https://docs.gitlab.com/ee/topics/gitlab_flow.html#production-branch-with-gitlab-flow)
