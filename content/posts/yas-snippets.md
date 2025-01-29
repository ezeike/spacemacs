+++
title = "YAS snippets"
author = ["Eric Nielson"]
draft = false
+++

git clone <https://github.com/atotto/yasnippet-golang.git>

| Function       | Description         |
|----------------|---------------------|
| yas-reload-all | Reload all snippets |


## Shortcuts {#shortcuts}

<div class="ox-hugo-table my-table">
<div class="table-caption">
  <span class="table-number">Table 1:</span>
  Shortcut keys for development
</div>

| Keys  | Description  |
|-------|--------------|
| mod / | autocomplete |

</div>


## org mode snippets {#org-mode-snippets}

sb source block

```shell
yay -S nix
systemctl enable nix-daemon.service
gpasswd -a enielson nix-users
```

```shell
nix-channel --add https://nixos.org/channels/nixpkgs-unstable
nix-channel --update
```
