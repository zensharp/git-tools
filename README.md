# Overview
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
```
$ git publish [-c|--create [-a|--merge-when-pipeline-succeeds]]
```

| Option | Description |
| --- | --- |
| `create` | Creates a merge request for this branch. The merge request details are formatted for [automatic issue closing](https://docs.gitlab.com/ee/user/project/issues/managing_issues.html#closing-issues-automatically). |
| `merge-when-pipeline-succeeds` | Automatically merges the merge request if the pipeline succeeds. |

> See [GitLab push options](https://docs.gitlab.com/ee/user/project/push_options.html) for more information.

## Git Feature (Experimental)
* Manages feature branches.
```
$ git feature start foo
$ git feature drop foo
$ git feature prune
```

## Git Sweep (Experimental)
* Synchronizes the local repository with the remote.

# Installation
1. Place these scripts in a persistent location.
2. Add the location to `PATH`.
