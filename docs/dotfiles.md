---
icon: simple/gnubash
tags:
    - evergreen
    - uses
---

# dotfiles <span class="caret"></span>

<div class="grid cards" markdown>

- :octicons-git-branch-16:{ .foreground } [tylernguyen/dotfiles :octicons-arrow-up-right-16:](https://github.com/tylernguyen/dotfiles)
    ![GitHub Stars](https://img.shields.io/github/stars/tylernguyen/dotfiles?style=flat&logo=refinedgithub&logoColor=073642&labelColor=eee8d5&color=859900#only-light){ .twemoji }
    ![GitHub Last Commit](https://img.shields.io/github/last-commit/tylernguyen/dotfiles?style=flat&logo=refinedgithub&logoColor=073642&labelColor=eee8d5&color=859900#only-light){ .twemoji }
    ![GitHub Stars](https://img.shields.io/github/stars/tylernguyen/dotfiles?style=flat&logo=refinedgithub&logoColor=839496&labelColor=073642&color=2aa198#only-dark){ .twemoji }
    ![GitHub Last Commit](https://img.shields.io/github/last-commit/tylernguyen/dotfiles?style=flat&logo=refinedgithub&logoColor=839496&labelColor=073642&color=2aa198#only-dark){ .twemoji }

</div>

<div class="grid cards" markdown>

- ![chezmoi](https://assets.tylernguyen.wiki/logos/chezmoi.svg){ .twemoji } [chezmoi :octicons-arrow-up-right-16:](https://github.com/twpayne/chezmoi/)
[:octicons-markdown-16:](https://www.chezmoi.io/){ title=Documentation}
[:lucide-file-code-corner:](https://github.com/twpayne/chezmoi){ title="Source Code" }
[:lucide-scale:](https://github.com/twpayne/chezmoi/blob/master/LICENSE){ title=License }

    ``` bash

    chezmoi init --ssh tylernguyen

    ```

</div>

<div class="grid cards" markdown>

- :simple-1password:{ .onepassword } [1Password :octicons-arrow-up-right-16:](https://1password.com/)
[:lucide-circle-dollar-sign:](https://1password.com/sign-up/){ title=Pricing }
[:lucide-hat-glasses:](https://support.onepassword.com/1password-privacy/){ title="Privacy Policy" }
[:octicons-markdown-16:](https://developer.onepassword.com/){ title="Developer Documentation" }

- :simple-ghostty:{ .ghostty } [ghostty :octicons-arrow-up-right-16:](https://ghostty.org/)
[:octicons-markdown-16:](https://ghostty.org/docs){ title=Documentation}
[:lucide-file-code-corner:](https://github.com/ghostty-org/ghostty){ title="Source Code" }
[:lucide-scale:](https://github.com/ghostty-org/ghostty/blob/main/LICENSE){ title=License }

</div>

<div class="grid cards" markdown>

- :simple-zsh:{ .zsh } [zsh :octicons-arrow-up-right-16:](https://zsh.sourceforge.io/)
[:octicons-markdown-16:](https://zsh.sourceforge.io/Doc/){ title=Documentation}

    :octicons-git-branch-16:{ .foreground } [zimfw/zimfw :octicons-arrow-up-right-16:](<https://github.com/zimfw/zimfw>)
        ![GitHub Stars](https://img.shields.io/github/stars/zimfw/zimfw?style=flat&logo=refinedgithub&logoColor=073642&labelColor=eee8d5&color=859900#only-light){ .twemoji }
        ![GitHub Release Date](https://img.shields.io/github/release-date/zimfw/zimfw?style=flat&logo=refinedgithub&logoColor=073642&labelColor=eee8d5&color=859900#only-light){ .twemoji }
        ![GitHub Stars](https://img.shields.io/github/stars/zimfw/zimfw?style=flat&logo=refinedgithub&logoColor=839496&labelColor=073642&color=2aa198#only-dark){ .twemoji }
        ![GitHub Release Date](https://img.shields.io/github/release-date/zimfw/zimfw?style=flat&logo=refinedgithub&logoColor=839496&labelColor=073642&color=2aa198#only-dark){ .twemoji }

    :octicons-git-branch-16:{ .foreground } [atuinsh/atuin :octicons-arrow-up-right-16:](<https://github.com/atuinsh/atuin>)
        ![GitHub Stars](https://img.shields.io/github/stars/atuinsh/atuin?style=flat&logo=refinedgithub&logoColor=073642&labelColor=eee8d5&color=859900#only-light){ .twemoji }
        ![GitHub Release Date](https://img.shields.io/github/release-date/atuinsh/atuin?style=flat&logo=refinedgithub&logoColor=073642&labelColor=eee8d5&color=859900#only-light){ .twemoji }
        ![GitHub Stars](https://img.shields.io/github/stars/atuinsh/atuin?style=flat&logo=refinedgithub&logoColor=839496&labelColor=073642&color=2aa198#only-dark){ .twemoji }
        ![GitHub Release Date](https://img.shields.io/github/release-date/atuinsh/atuin?style=flat&logo=refinedgithub&logoColor=839496&labelColor=073642&color=2aa198#only-dark){ .twemoji }

    :octicons-git-branch-16:{ .foreground } [Aloxaf/fzf-tab :octicons-arrow-up-right-16:](https://github.com/Aloxaf/fzf-tab)
        ![GitHub Stars](https://img.shields.io/github/stars/Aloxaf/fzf-tab?style=flat&logo=refinedgithub&logoColor=073642&labelColor=eee8d5&color=859900#only-light){ .twemoji }
        ![GitHub Release Date](https://img.shields.io/github/release-date/Aloxaf/fzf-tab?style=flat&logo=refinedgithub&logoColor=073642&labelColor=eee8d5&color=859900#only-light){ .twemoji }
        ![GitHub Stars](https://img.shields.io/github/stars/Aloxaf/fzf-tab?style=flat&logo=refinedgithub&logoColor=839496&labelColor=073642&color=2aa198#only-dark){ .twemoji }
        ![GitHub Release Date](https://img.shields.io/github/release-date/Aloxaf/fzf-tab?style=flat&logo=refinedgithub&logoColor=839496&labelColor=073642&color=2aa198#only-dark){ .twemoji }

</div>

/// abstract
dotfiles is designed with maximum cross-platform compatibility, minimal components, and universal behaviors in mind.
///

## Git :simple-git:{ .git }

`.gitconfig` uses `code` (Visual Studio Code) as the editor, diff and merge tool.

1Password handles SSH authentication and signing.

Projects live under `src/` and are associated with their respective SSH signing key, i.e. `src/tylernguyen@GitHub`, `src/tylernguyen@GitLab`, `tylernguyen.codes`.

I prefer to rebase by default, unless there is very specific reason to merge.

## Package Managers

<div class="grid cards" markdown>

- :simple-gnubash:{ .gnubash } [winget :octicons-arrow-up-right-16:](https://github.com/microsoft/winget-cli)
- :simple-flatpak:{ .flatpak } [Flatpak :octicons-arrow-up-right-16:](<https://flatpak.org/>)
- :simple-homebrew:{ .homebrew } [homebrew :octicons-arrow-up-right-16:](https://brew.sh/)

</div>

/// note

On Windows, portable executables are placed in `%userprofile%/bin`. Include this in `PATH`.

///
