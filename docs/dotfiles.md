---
icon: simple/gnubash
tags:
    - evergreen
    - uses
---

# dotfiles <span class="caret"></span>

## [tylernguyen/dotfiles :lucide-arrow-up-right:](https://github.com/tylernguyen/dotfiles)

I intentionally keep my dotfiles bare and basic. Its sole purpose is to intialize my CLI, secrets, and SSH workflow. Other application settings are backed up separately.

- ![chezmoi](https://assets.tylernguyen.wiki/logos/chezmoi.svg){ .twemoji } [chezmoi :lucide-arrow-up-right:](https://github.com/twpayne/chezmoi/) manages the dotfiles.
  [:octicons-markdown-16:](https://www.chezmoi.io/){ title=Documentation}
  [:lucide-scale:](https://github.com/twpayne/chezmoi/blob/master/LICENSE){ title=License }
- :simple-1password:{ .onepassword } [1Password :lucide-arrow-up-right:](https://1password.com/) is my secrets and SSH manager.
  [:lucide-circle-dollar-sign:](https://1password.com/sign-up/){ title=Pricing }
  [:lucide-hat-glasses:](https://support.onepassword.com/1password-privacy/){ title="Privacy Policy" }
- :simple-zsh:{ .zsh } [z shell :lucide-arrow-up-right:](https://zsh.sourceforge.io/)
  [:octicons-markdown-16:](https://zsh.sourceforge.io/Doc/){ title=Documentation}
    - ![atuin](https://assets.tylernguyen.wiki/logos/atuin.svg){ .twemoji }  [atuinsh/atuin :lucide-arrow-up-right:](<https://github.com/atuinsh/atuin>)
    - :lucide-folder-git-2:{ .foreground } [zimfw/zimfw :lucide-arrow-up-right:](<https://github.com/zimfw/zimfw>)
    - :lucide-folder-git-2:{ .foreground } [Aloxaf/fzf-tab :lucide-arrow-up-right:](https://github.com/Aloxaf/fzf-tab)

- :simple-ghostty:{ .ghostty } [ghostty :lucide-arrow-up-right:](https://ghostty.org/)
  [:octicons-markdown-16:](https://ghostty.org/docs){ title=Documentation}
  [:lucide-file-code-corner:](https://github.com/ghostty-org/ghostty){ title="Source Code" }
  [:lucide-scale:](https://github.com/ghostty-org/ghostty/blob/main/LICENSE){ title=License }

## Git :simple-git:{ .git }

`.gitconfig` uses `code` (Visual Studio Code) as the editor, diff and merge tool.

Projects live under `src/` and are associated with their respective SSH signing key, i.e. `src/tylernguyen@GitHub`, `src/tylernguyen@GitLab`, `tylernguyen.codes`.

I prefer to rebase by default, unless there is very specific reason to merge.

## Package Managers

- :simple-gnubash:{ .gnubash } [winget :lucide-arrow-up-right:](https://github.com/microsoft/winget-cli)

> [!note]
> On Windows, portable executables are placed in `%userprofile%/bin`. Include this in `PATH`.

- :simple-homebrew:{ .homebrew } [homebrew :lucide-arrow-up-right:](https://brew.sh/)
- :simple-flatpak:{ .flatpak } [Flatpak :lucide-arrow-up-right:](<https://flatpak.org/>)
