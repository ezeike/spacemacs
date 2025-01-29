+++
author = ["Eric Nielson"]
draft = false
+++

Press `SPC g s` to get into git status.

`d d` on a commit to view the changes


## Shortcuts {#shortcuts}

<div class="ox-hugo-table my-table">
<div class="table-caption">
  <span class="table-number">Table 1:</span>
  Shortcut keys for development
</div>

| Keys        | Function  | Description                                           |
|-------------|-----------|-------------------------------------------------------|
| SPC g s d d |           | Diff between local and remote (type master in prompt) |
| SPC g s b x |           | Delete a branch                                       |
| SPC g b     | Git blame | Git blame                                             |

</div>


## Adding existing project to gitlab {#adding-existing-project-to-gitlab}

SPC g i    git init

```shell
git remote add origin git@gitlab10:enielson/project.git
git push -u origin master
```


### Reviewing PRs {#reviewing-prs}

SPC g b


## Git pull/fetch merging master into current branch {#git-pull-fetch-merging-master-into-current-branch}


#### Git fetch downloads remote changes but does not make any local changes {#git-fetch-downloads-remote-changes-but-does-not-make-any-local-changes}


#### Git pull is a git fetch followed by git merge {#git-pull-is-a-git-fetch-followed-by-git-merge}
