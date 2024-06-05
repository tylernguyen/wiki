---
icon: material/signal-cellular-outline
tags:
  - Evergreen
---

# Services

I hate subscriptions and actively avoid them when I can. This is mostly a financial decision but is also motivated by data privacy. The services here are mostly irreplaceable for their features and/or should not be self-hosted for security.

## Productivity

<div class="grid cards" markdown>

- :simple-todoist:{ .todoist } [Todoist](https://todoist.com/)

</div>

## Media

<div class="grid cards" markdown>

- :simple-audible:{ .audible } [Audible](https://www.audible.com/)
- :simple-pocketcasts:{ .pocketcasts } [Pocket Casts](https://pocketcasts.com/)
- ![Libby](https://assets.tylernguyen.wiki/logos/Libby.png){ .twemoji } [Libby](https://libbyapp.com)

</div>

/// warning
Audible is a subsidiary of Amazon.[^1]

Audible is only used for exclusives.

eBooks and audiobooks are sold by Amazon with DRM. Buy directly from publisher and your local bookstore when possible!
///

/// tip
Consider archiving your audiobooks from Audible. See [rmcrackan/Libation](https://github.com/rmcrackan/Libation).
///

## 1Password

<div class="grid cards" markdown>

- <figure markdown>
    <p align="center">
    ![1Password](https://assets.tylernguyen.wiki/logos/1Password-light.svg#only-light){ width=200 }
    ![1Password](https://assets.tylernguyen.wiki/logos/1Password-dark.svg#only-dark){ width=200 }
    </p>
    </figure>

</div>

/// warning
1Password is not open source.
///

1Password is robust, cross-platform, and well integrated. Its ease of use and wide adoption also makes sharing passwords effortless.

1Password also offers various developer functions that I find cannot be matched by other offerings. These include:

- SSH Authentication
- Git Commit Signing
- Developer Tokens and Secrets Automation
- [twpayne/chezmoi](https://www.chezmoi.io/user-guide/password-managers/1password/) integration for managing dotfiles
- [Visual Studio Code](https://developer.1password.com/docs/vscode/) integration for editing secrets

/// info
1Password is [audited](https://support.onepassword.com/security-assessments/) on a regular basis and also documents their security in the [security white paper](https://1passwordstatic.com/files/security/1password-white-paper.pdf).
///

[:octicons-link-external-16: Homepage](https://1password.com/){ .md-button }
[:fontawesome-solid-money-bill:](https://1password.com/sign-up/){ .card-link title=Pricing }
[:fontawesome-regular-eye:](https://support.onepassword.com/1password-privacy/){ .card-link title="Privacy Policy" }
[:octicons-markdown-16:](https://developer.onepassword.com/){ .card-link title="Developer Documentation" }

## Proton Unlimited

<div class="grid cards" markdown>

- <figure markdown>
    <p align="center">
    ![Proton](https://assets.tylernguyen.wiki/logos/Proton-logotype-purple-noborder.svg){ width=200 }
    </p>
    </figure>

</div>

<div class="grid cards" markdown>

- :simple-protonmail:{ .protonmail } [ProtonMail](https://protonmail.com/)

    /// warning
    Email is an insecure form of communication by design. [^2]
    ///

</div>

<div class="grid cards" markdown>

- :simple-protonvpn:{ .protonvpn } [Proton VPN](https://protonvpn.com/)

    I use ProtonVPN purely for P2P traffic as it's one of the few VPN services that supports [port forwarding](https://protonvpn.com/blog/port-forwarding/).

    /// danger
    VPNs do not provide anonymity.[^3]
    ///

</div>

<div class="grid cards" markdown>

- :simple-protondrive:{ .protondrive } [ProtonDrive](https://proton.me/drive)
- :simple-simplelogin:{ .simplelogin } [SimpleLogin](https://simplelogin.io/)

</div>

[:octicons-link-external-16: Homepage](https://proton.me/){ .md-button }
[:simple-torbrowser:{.torproject }](http://o54hon2e2vj6c7m3aqqu6uyece65by3vgoxxhlqlsvkmacw6a7m7kiad.onion){ .card-link title="Onion Service" }
[:fontawesome-solid-money-bill:](https://proton.me/pricing){ .card-link title="Pricing" }
[:fontawesome-regular-eye:](https://proton.me/legal/privacy){ .card-link title="Privacy Policy" }
[:octicons-markdown-16:](https://mullvad.net/en/help/){ .card-link title=Documentation }

## Cloudflare

<div class="grid cards" markdown>

- :simple-cloudflare:{ .cloudflare } [Cloudflare Domain Registar](https://www.cloudflare.com/products/registrar/)

    Cloudflare offers at-cost pricing both for new registrations and renewals.

- :simple-cloudflare:{ .cloudflare } [Cloudflare DNS](https://www.cloudflare.com/)
- :simple-cloudflare:{ .cloudflare } [Cloudflare R2](https://www.cloudflare.com/products/r2/)

    Cloudflare R2 hosts assets for this wiki, as well as for my [Mastodon instance](https://tylernguyen.social/@tylernguyen).

- ![Cloudflare Workers](https://assets.tylernguyen.wiki/logos/Cloudflare-Workers.png){ .twemoji } [Cloudflare Workers](https://workers.cloudflare.com/)
- :simple-cloudflarepages:{ .cloudflarepages } [Cloudflare Pages](https://pages.cloudflare.com/)
- ![Cloudflare Zero Trust](https://assets.tylernguyen.wiki/logos/Cloudflare-Zero-Trust.svg){ .twemoji } [Cloudflare Zero Trust](https://www.cloudflare.com/zero-trust/)

</div>

[:octicons-link-external-16: Homepage](https://cloudflare.com/){ .md-button }
[:fontawesome-regular-eye:](https://www.cloudflare.com/privacypolicy/){ .card-link title="Privacy Policy" }
[:octicons-markdown-16:](https://developers.cloudflare.com/){ .card-link title=Documentation }
[:octicons-typography-16:](https://blog.cloudflare.com/){ .card-link title=Blog }

## Postmark

<div class="grid cards" markdown>

- ![Postmark](https://assets.tylernguyen.wiki/logos/Postmark.png){ .twemoji } [Postmark](https://postmarkapp.com/)

</div>

I mainly need transactional email for self-hosted apps, which send a very low volume. Postmark's free plan has been perfect for this.

[:octicons-link-external-16: Homepage](https://postmarkapp.com/){ .md-button }
[:fontawesome-solid-money-bill:](https://postmarkapp.com/pricing){ .card-link title="Pricing" }
[:fontawesome-regular-eye:](https://postmarkapp.com/privacy-policy){ .card-link title="Privacy Policy" }
[:octicons-markdown-16:](https://postmarkapp.com/manual){ .card-link title=Documentation }

[^1]: [Richard Stallman: Reasons not to buy from Amazon](https://stallman.org/amazon.html)
[^2]: [Privacy Guides: Email is an insecure form of communication by default](https://www.privacyguides.org/basics/email-security/)
[^3]: [Privacy Guides: VPN Overview](https://www.privacyguides.org/vpn/#vpn-overview)
