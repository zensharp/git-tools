# Installation
1. Place these scripts in a persistent location.
2. Add the location to `PATH`.

## Git Browse
* Opens the repository in your default web browser. Note: only GitHub, GitLab, and BitBucket remotes are supported.

> The environment variable `BROWSER` must be set.

## Git Lazy
* Commits and pushes all modified + untracked files.

## Git Produce
* Creates (or updates) a production branch from master. Then pushes the branch.
	* See [GitLab Flow](https://docs.gitlab.com/ee/topics/gitlab_flow.html#production-branch-with-gitlab-flow)
	
## Git Publish
* Pushes the branch to `origin` and sets up remote tracking.

## Git Feature (Experimental)
* Manages feature branches.
```
$ git feature start x
$ git feature drop x
$ git feature prune
```

> The feature branches will be created with the name `feature/x` where `x` is the name provided in `git feature start`.

## Git Sweep (Experimental)
* Synchronizes the local repository with the remote.
