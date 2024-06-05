---
  icon: simple/gnubash
---

# dotfiles

<div style="text-align:center;" markdown>

[:octicons-repo-16:{ .github } github.com/tylernguyen/dotfiles](https://github.com/tylernguyen/dotfiles){ .md-button }

</div>

/// abstract
dotfiles is designed with maximum cross-platform compatibility, minimal components, and universal behaviors in mind.
///

/// extension | Components
<div class="grid cards" markdown>

- ![zsh](https://assets.tylernguyen.wiki/logos/zsh.svg){ .twemoji } [zsh](https://zsh.sourceforge.io/)
[:octicons-markdown-16:](https://zsh.sourceforge.io/Doc/){ .card-link title=Documentation}

- ![chezmoi](https://assets.tylernguyen.wiki/logos/chezmoi.svg){ .twemoji } [chezmoi](https://github.com/twpayne/chezmoi/)
[:octicons-markdown-16:](https://www.chezmoi.io/){ .card-link title=Documentation}
[:fontawesome-regular-file-code:](https://github.com/twpayne/chezmoi){ .card-link title="Source Code" }
[:octicons-law-16:](https://github.com/twpayne/chezmoi/blob/master/LICENSE){ .card-link title=License }

- :simple-wezterm:{ .wezterm } [wezterm](https://wezfurlong.org/wezterm/index.html)
[:octicons-markdown-16:](https://wezfurlong.org/wezterm/){ .card-link title=Documentation}
[:fontawesome-regular-file-code:](https://github.com/wez/wezterm){ .card-link title="Source Code" }
[:octicons-law-16:](https://github.com/wez/wezterm/blob/main/LICENSE.md){ .card-link title=License }

- :simple-1password:{ .onepassword } [1Password](https://1password.com/)
[:fontawesome-solid-money-bill:](https://1password.com/sign-up/){ .card-link title=Pricing }
[:fontawesome-regular-eye:](https://support.onepassword.com/1password-privacy/){ .card-link title="Privacy Policy" }
[:octicons-markdown-16:](https://developer.onepassword.com/){ .card-link title="Developer Documentation" }

</div>
///

## Wezterm :simple-wezterm:{ .wezterm }

- Cross-platform, written in Rust
- [GPU-accelerated](https://wezfurlong.org/wezterm/config/lua/config/front_end.html)
- Ligature support
- [Nerd Fonts fallback](https://wezfurlong.org/wezterm/config/lua/wezterm/nerdfonts.html)

## Z Shell ![zsh](https://assets.tylernguyen.wiki/logos/zsh.svg){ .twemoji }

- :octicons-repo-16:{ .github } [zimfw/zimfw](<https://github.com/zimfw/zimfw>) - Plugin Manager
- :octicons-repo-16:{ .github } [romkatv/powerlevel10k](<https://github.com/romkatv/powerlevel10k>) - Prompt Theme
- :octicons-repo-16:{ .github } [atunish/atuin](<https://github.com/atuinsh/atuin>) - Shell History TUI
- :octicons-repo-16:{ .github } [Aloxaf/fzf-tab](https://github.com/Aloxaf/fzf-tab) - fzf Completion Menu

## Git :simple-git:{ .git }

`.gitconfig` uses `code` (Visual Studio Code) as the editor, diff and merge tool.

1Password handles SSH authentication and signing.

Projects live under `src/` and are associated with their respective SSH signing key, i.e. `src/tylernguyen@GitHub`, `src/tylernguyen@GitLab`, `tylernguyen.codes`

I prefer to rebase by default, unless there is very specific reason to merge.

## Package Managers

On Windows :simple-windows:{ .windows } , I use `winget` by default, supplementing it with third-party installers and the Microsoft Store if needed. Portable executables are placed in `%userprofile%/bin`.

On macOS :simple-apple:{ .apple } , [:simple-homebrew:{ .homebrew } homebrew](https://brew.sh/) is preferred and likewise supplemented by the App Store.

Depending on the Linux :simple-linux:{ .linux } distribution, I tend to use the default package managers such `apt` or `pacman`. If there are no feature difference, however, I will defer to installation via [:simple-flatpak:{ .flatpak } flatpak](https://flatpak.org/).
