---
icon: simple/gnubash
tags:
    - evergreen
    - uses
---

# dotfiles

## [tylernguyen/dotfiles :lucide-arrow-up-right:](https://github.com/tylernguyen/dotfiles)

I intentionally keep my dotfiles bare and basic. Its sole purpose is to intialize my CLI, secrets, and SSH workflow. Other application settings are backed up separately.

- ![chezmoi](https://assets.tylernguyen.wiki/logos/chezmoi.svg){ .twemoji } [chezmoi :lucide-arrow-up-right:](https://github.com/twpayne/chezmoi/) as dotfiles manager.
  [:lucide-file-text:](https://www.chezmoi.io/){ .extra title=Documentation}
- :simple-1password:{ .onepassword } [1Password :lucide-arrow-up-right:](https://1password.com/) as SSH and secrets manager.
  [:lucide-circle-dollar-sign:](https://1password.com/sign-up/){ .extra title=Pricing }
  [:lucide-hat-glasses:](https://support.onepassword.com/1password-privacy/){ .extra title="Privacy Policy" }
- :simple-zsh:{ .zsh } [z shell :lucide-arrow-up-right:](https://zsh.sourceforge.io/)
  [:lucide-file-text:](https://zsh.sourceforge.io/Doc/){ .extra title=Documentation}
    - ![atuin](https://assets.tylernguyen.wiki/logos/atuin.svg){ .twemoji }  [atuinsh/atuin :lucide-arrow-up-right:](<https://github.com/atuinsh/atuin>)
    - :lucide-folder-git-2:{ .foreground } [zimfw/zimfw :lucide-arrow-up-right:](<https://github.com/zimfw/zimfw>)
    - :lucide-folder-git-2:{ .foreground } [Aloxaf/fzf-tab :lucide-arrow-up-right:](https://github.com/Aloxaf/fzf-tab)

- :simple-ghostty:{ .ghostty } [ghostty :lucide-arrow-up-right:](https://ghostty.org/)
  [:lucide-file-text:](https://ghostty.org/docs){ .extra title=Documentation}
  [:lucide-file-code-corner:](https://github.com/ghostty-org/ghostty){ .extra title="Source Code" }
  [:lucide-scale:](https://github.com/ghostty-org/ghostty/blob/main/LICENSE){ .extra title=License }

```
~/
├─ src/
│  ├─ tylernguyen@GitHub/
│  │  ├─ wiki/
│  │  ├─ pymdownx-mahjong/
│  │  ├─ ...
│  ├─ tylernguyen.codes/
│  ├─ ...
├─ .gitconfig
├─ .tylernguyen@GitHub.gitconfig
├─ .tylernguyen.codes.gitconfig
├─ ...
```

Projects live under `~/src/`, organized by the SSH key they are associated with.

## Package Managers

- :simple-gnubash:{ .gnubash } [winget :lucide-arrow-up-right:](https://github.com/microsoft/winget-cli)

> [!note]
> On Windows, portable executables are placed in `%userprofile%/bin`. Include this in `PATH`.

- :simple-homebrew:{ .homebrew } [homebrew :lucide-arrow-up-right:](https://brew.sh/)
- :simple-flatpak:{ .flatpak } [Flatpak :lucide-arrow-up-right:](<https://flatpak.org/>)
