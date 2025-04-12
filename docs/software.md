---
icon: octicons/apps-16
tags:
  - Evergreen
---

# Software

Though I do prefer free (as in freedom) software, I do use proprietary software if its open-source alternative is not adequate.

## 1Password

<div class="grid cards" markdown>

- <figure markdown>
    <p align="center">
    ![1Password](https://assets.tylernguyen.wiki/logos/1Password-light.svg#only-light){ loading-lazy width=200 }
    ![1Password](https://assets.tylernguyen.wiki/logos/1Password-dark.svg#only-dark){ loading-lazy width=200 }
    </p>
    </figure>

</div>

/// info
1Password is a <span class="solarized-red">:material-lock: __proprietary__</span>, <span class="solarized-green">:material-sync: __subscription__</span>-ware password manager.
///

1Password is robust, cross-platform, and well integrated. Its ease of use and wide adoption also makes sharing passwords effortless.

1Password also offers various developer functions that I find cannot be matched by other offerings. These include:

- SSH Authentication
- Git Commit Signing
- Developer Tokens and Secrets Automation
- [:octicons-git-branch-16:{ .foreground } twpayne/chezmoi :octicons-arrow-up-right-16:](https://www.chezmoi.io/user-guide/password-managers/1password/) integration for managing dotfiles
- [Visual Studio Code](https://developer.1password.com/docs/vscode/) integration for editing secrets

/// success | Security
1Password is [audited](https://support.onepassword.com/security-assessments/) on a regular basis and also documents their security in the [security white paper](https://1passwordstatic.com/files/security/1password-white-paper.pdf).
///

[Homepage :octicons-arrow-up-right-16:](https://1password.com/){ .md-button }
[:fontawesome-solid-money-bill:](https://1password.com/sign-up/){ .card-link title=Pricing }
[:fontawesome-regular-eye:](https://support.onepassword.com/1password-privacy/){ .card-link title="Privacy Policy" }
[:octicons-markdown-16:](https://developer.onepassword.com/){ .card-link title="Developer Documentation" }

## Firefox

<div class="grid cards" markdown>

- <figure markdown>
    <p align="center">
    ![Firefox](https://assets.tylernguyen.wiki/logos/Firefox-light.svg#only-light){ loading-lazy width=200 }
    ![Firefox](https://assets.tylernguyen.wiki/logos/Firefox-dark.svg#only-dark){ loading-lazy width=200 }
    </p>
    </figure>

</div>

/// info
Firefox is an <span class="solarized-orange">:material-source-branch: __open source__</span> web browser.
///

/// extension | Extensions
<div class="grid cards" markdown>

- :simple-ublockorigin:{ .ublockorigin } [uBlock Origin :octicons-arrow-up-right-16:](https://addons.mozilla.org/en-US/firefox/addon/ublock-origin/) [^1]
[:fontawesome-regular-file-code:](https://github.com/gorhill/uBlock){ .card-link title="Source Code" }
- ![SponsorBlock](https://assets.tylernguyen.wiki/logos/Firefox_SponsorBlock.png){ .twemoji } [SponsorBlock :octicons-arrow-up-right-16:](https://addons.mozilla.org/en-US/firefox/addon/sponsorblock/)
- ![TTV LOL Pro](https://assets.tylernguyen.wiki/logos/Firefox_TTV-LOL-Pro.png){ .twemoji } [TTV LOL Pro :octicons-arrow-up-right-16:](https://addons.mozilla.org/en-US/firefox/addon/ttv-lol-pro/?utm_source=addons.mozilla.org&utm_medium=referral&utm_content=search)
[:fontawesome-regular-file-code:](https://github.com/younesaassila/ttv-lol-pro){ .card-link title="Source Code" }
- :simple-1password:{ .onepassword } [1Password :octicons-arrow-up-right-16:](https://addons.mozilla.org/en-US/firefox/addon/1password-x-password-manager/)

</div>
///

[^1]: [gorhill/uBlock: uBlock Origin Works Best on Firefox](https://github.com/gorhill/uBlock/wiki/uBlock-Origin-works-best-on-Firefox)

[Homepage :octicons-arrow-up-right-16:](https://firefox.com){ .md-button }
[:fontawesome-regular-eye:](https://www.mozilla.org/privacy/firefox/){ .card-link title="Privacy Policy" }
[:octicons-markdown-16:](https://firefox-source-docs.mozilla.org/){ .card-link title=Documentation}
[:fontawesome-regular-file-code:](https://hg.mozilla.org/mozilla-central){ .card-link title="Source Code" }
[:fontawesome-regular-heart:](https://donate.mozilla.org/){ .card-link title=Contribute }

## Visual Studio Code

<div class="grid cards" markdown>

- <figure markdown>
    <p align="center">
    ![Visual Studio Code](https://assets.tylernguyen.wiki/logos/VSCode.svg#only-light){ loading-lazy width=100 }
    ![Visual Studio Code](https://assets.tylernguyen.wiki/logos/VSCode-dark.svg#only-dark){ loading-lazy width=100 }
    </p>
    </figure>

</div>

I use Visual Studio Code is mainly for extensions and remote capabilities.

//// collapse-code

```json title="settings.json"

--8<-- "https://gist.githubusercontent.com/tylernguyen/fd3271d4d2ab037e9a4bd43270866684/raw/b65f342c04b88800e16f0bdf8929ea51805af041/vscode_settings.json"

```

////

/// extension | Extensions

<div class="grid cards" markdown>

- ![Fluent Icons](https://assets.tylernguyen.wiki/logos/VSCode_Fluent-Icons.png){ .twemoji } [Fluent Icons :octicons-arrow-up-right-16:](https://marketplace.visualstudio.com/items?itemName=miguelsolorio.fluent-icons)
- ![Comment Anchors](https://assets.tylernguyen.wiki/logos/VSCode_Comment-Anchors.png){ .twemoji } [Comment Anchors :octicons-arrow-up-right-16:](https://marketplace.visualstudio.com/items?itemName=ExodiusStudios.comment-anchors)
- ![GitHub Repositories](https://assets.tylernguyen.wiki/logos/VSCode_GitHub-Repositories.png){ .twemoji } [GitHub Repositories :octicons-arrow-up-right-16:](https://marketplace.visualstudio.com/items?itemName=GitHub.remotehub)
- ![GitHub Actions](https://assets.tylernguyen.wiki/logos/VSCode_GitHub-Actions.png){ .twemoji } [GitHub Actions :octicons-arrow-up-right-16:](https://marketplace.visualstudio.com/items?itemName=GitHub.vscode-github-actions)
- ![Block Sort](https://assets.tylernguyen.wiki/logos/VSCode_Block-Sort.png){ .twemoji } [Block Sort :octicons-arrow-up-right-16:](https://marketplace.visualstudio.com/items?itemName=1nVitr0.blocksort)
- :simple-1password:{ .onepassword } [1Password :octicons-arrow-up-right-16:](https://marketplace.visualstudio.com/items?itemName=1Password.op-vscode)
- ![Error Lens](https://assets.tylernguyen.wiki/logos/VSCode_Error-Lens.png){ .twemoji } [Error Lens :octicons-arrow-up-right-16:](https://marketplace.visualstudio.com/items?itemName=usernamehw.errorlens)
- ![Tailscale](https://assets.tylernguyen.wiki/logos/Tailscale.png){ .twemoji } [Tailscale :octicons-arrow-up-right-16:](https://marketplace.visualstudio.com/items?itemName=Tailscale.vscode-tailscale)
- :simple-docker:{ .docker } [Docker :octicons-arrow-up-right-16:](https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-docker)

</div>
///

[Homepage :octicons-arrow-up-right-16:](https://code.visualstudio.com/){ .md-button }
[:fontawesome-regular-eye:](https://privacy.microsoft.com/en-US/privacystatement){ .card-link title="Privacy Policy" }
[:octicons-markdown-16:](https://code.visualstudio.com/docs){ .card-link title=Documentation}
[:fontawesome-regular-file-code:](https://github.com/microsoft/vscode){ .card-link title="Source Code" }

## Material for MkDocs

<div class="grid cards" markdown>

- :simple-materialformkdocs:{ .materialformkdocs } [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) [*Insiders*](https://squidfunk.github.io/mkdocs-material/insiders/)
[:fontawesome-solid-money-bill:](https://github.com/sponsors/squidfunk){ .card-link title="Pricing" }
[:fontawesome-regular-file-code:](https://github.com/squidfunk/mkdocs-material){ .card-link title="Source Code" }
[:octicons-law-16:](https://github.com/squidfunk/mkdocs-material/blob/master/LICENSE){ .card-link title=License }

</div>

/// info
Material for MkDocs is a <span class="solarized-green">:material-sync: __sponsor__</span>-ware, <span class="solarized-orange">:material-source-branch: __open source__</span> static site generator intended for documentation. Sponsoring the project grants access to a private development fork called Insiders.
///

/// example
This website is created using Material for MkDocs Insiders.
///

## Virtualization

<div class="grid cards" markdown>

- :simple-docker:{ .docker } [Docker Desktop :octicons-arrow-up-right-16:](https://www.docker.com/products/docker-desktop/)
[:fontawesome-solid-money-bill:](https://www.docker.com/pricing/){ .card-link title="Pricing" }
- ![OrbStack](https://assets.tylernguyen.wiki/logos/OrbStack.png){ .twemoji } [OrbStack :octicons-arrow-up-right-16:](https://orbstack.dev/)
[:fontawesome-solid-money-bill:](https://orbstack.dev/pricing){ .card-link title="Pricing" }

</div>

## Media

<div class="grid cards" markdown>

- ![NetNewsWire](https://assets.tylernguyen.wiki/logos/NetNewsWire.png){ .twemoji } [NetNewsWire :octicons-arrow-up-right-16:](https://netnewswire.com/)
- ![Plexamp](https://assets.tylernguyen.wiki/logos/Plexamp.png){ .twemoji } [Plexamp :octicons-arrow-up-right-16:](https://plexamp.com/)
- :simple-vlcmediaplayer:{ .vlc } [VLC Media Player :octicons-arrow-up-right-16:](https://www.videolan.org/vlc/)
- ![OBS](https://assets.tylernguyen.wiki/logos/OBS.svg){ .twemoji } [OBS Studio :octicons-arrow-up-right-16:](https://obsproject.com/)
[:fontawesome-regular-file-code:](https://github.com/obsproject/obs-studio "Source Code"){ .card-link }

</div>

## Files

<div class="grid cards" markdown>

- ![Mountain Duck](https://assets.tylernguyen.wiki/logos/Mountain-Duck.png){ .twemoji } [Mountain Duck :octicons-arrow-up-right-16:](https://mountainduck.io/)
- :simple-cryptomator:{ .cryptomator} [Cryptomator :octicons-arrow-up-right-16:](https://cryptomator.org/)
- ![Syncthing](https://assets.tylernguyen.wiki/logos/Syncthing.svg){ .twemoji } [Syncthing :octicons-arrow-up-right-16:](https://syncthing.net/)
[:fontawesome-regular-file-code:](https://github.com/syncthing/ "Source Code"){ .card-link }
[:octicons-markdown-16:](https://docs.syncthing.net/ "Documentation"){ .card-link }

</div>
