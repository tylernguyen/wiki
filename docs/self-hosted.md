---
icon: material/server-network-outline
tags:
  - Evergreen
---

# Self-Hosted

## Unraid

![Unraid](https://assets.tylernguyen.wiki/logos/Unraid-light.svg#only-light){ align=right width=150 }
![Unraid](https://assets.tylernguyen.wiki/logos/Unraid-dark.svg#only-dark){ align=right width=150 }

Unraid has a robust redundancy system, supports virtualization, third-party plugins, and Docker. Its UI and UX is straight forward and user-friendly.

The Unraid community is also very active and helpful.

/// warning
Unraid is not open source.
///

[:octicons-link-external-16: Homepage](https://unraid.net/){ .md-button }
[:fontawesome-solid-money-bill:](https://unraid.net/pricing){ .card-link title=Pricing}
[:octicons-markdown-16:](https://wiki.unraid.net/Documentation){ .card-link title=Documentation}

## Containers

/// note
I recommend the linuxserver Docker image for its [image mods](https://mods.linuxserver.io/?mod=plex).
///

<div class="grid cards" markdown>

- ![plex](https://assets.tylernguyen.wiki/logos/plex.svg){ .twemoji } [Plex Media Server](https://www.plex.tv/)
[:octicons-container-16:{ .docker }](https://hub.docker.com/r/linuxserver/plex){ .card-link title=Container}

- ![Audiobookshelf](https://assets.tylernguyen.wiki/logos/audiobookshelf.svg){ .twemoji } [Audiobookshelf](https://www.audiobookshelf.org/)
[:octicons-container-16:{ .docker }](https://github.com/advplyr/audiobookshelf/pkgs/container/audiobookshelf){ .card-link title=Container}
[:fontawesome-regular-file-code:](https://github.com/advplyr/audiobookshelf){ .card-link title="Source Code" }

- [:simple-gitea: Gitea](https://gitea.io/en-us/)
[:octicons-container-16:{ .docker }](https://hub.docker.com/r/gitea/gitea/tags){ .card-link title=Container}

- ![Paperless-ngx](https://assets.tylernguyen.wiki/logos/paperless-ngx.svg){ .twemoji } [Paperless-ngx](https://github.com/paperless-ngx/paperless-ngx)
[:octicons-container-16:{ .docker }](https://github.com/paperless-ngx/paperless-ngx/pkgs/container/paperless-ngx){ .card-link title=Container}
[:fontawesome-regular-file-code:](https://github.com/paperless-ngx/paperless-ngx){ .card-link title="Source Code" }

- ![Calibre](https://assets.tylernguyen.wiki/logos/calibre.svg){ .twemoji } [Calibre](https://calibre-ebook.com/)
[:octicons-container-16:{ .docker }](https://hub.docker.com/r/linuxserver/calibre){ .card-link title=Container}

- ![Kavita](https://assets.tylernguyen.wiki/logos/kavita.svg){ .twemoji } [Kavita](https://www.kavitareader.com/)
[:octicons-container-16:{ .docker }](https://hub.docker.com/r/linuxserver/kavita){ .card-link title=Container}
[:fontawesome-regular-file-code:](https://github.com/Kareadita/Kavita){ .card-link title="Source Code" }

- ![FreshRSS](https://assets.tylernguyen.wiki/logos/freshrss.svg){ .twemoji } [FreshRSS](https://freshrss.org/)
[:octicons-container-16:{ .docker }](https://hub.docker.com/r/linuxserver/freshrss){ .card-link title=Container}
[:fontawesome-regular-file-code:](https://github.com/FreshRSS/FreshRSS){ .card-link title="Source Code" }

- ![Kometa](https://assets.tylernguyen.wiki/logos/Kometa.png){ .twemoji } [Kometa (formerly plex-meta-manager)](https://github.com/meisnate12/Plex-Meta-Manager)
[:octicons-container-16:{ .docker }](https://hub.docker.com/r/kometateam/kometa){ .card-link title=Container}
[:fontawesome-regular-file-code:](https://github.com/Kometa-Team/Kometa){ .card-link title="Source Code" }

- ![Kometa/ImageMaid](https://assets.tylernguyen.wiki/logos/Kometa.png){ .twemoji } [Kometa/ImageMaid](https://github.com/meisnate12/Plex-Meta-Manager)
[:octicons-container-16:{ .docker }](https://hub.docker.com/r/kometateam/imagemaid){ .card-link title=Container}

- [giorgi-o/SkinPeek](https://github.com/giorgi-o/SkinPeek)
[:octicons-container-16:{ .docker }](https://github.com/users/giorgi-o/packages/container/package/skinpeek%2Fskinpeek){ .card-link title=Container}
[:fontawesome-regular-file-code:](https://github.com/giorgi-o/SkinPeek){ .card-link title="Source Code" }

- ![rmcrackan/Libation](https://assets.tylernguyen.wiki/logos/libation.png){ .twemoji } [rmcrackan/Libation](https://github.com/rmcrackan/Libation)
[:octicons-container-16:{ .docker }](https://hub.docker.com/r/rmcrackan/libation/tags){ .card-link title=Container}
[:fontawesome-regular-file-code:](https://github.com/rmcrackan/Libation){ .card-link title="Source Code" }

</div>

<div class="grid cards" markdown>

- :simple-mastodon:{ .mastodon } [Mastodon](https://joinmastodon.org/)
[:octicons-container-16:{ .docker }](https://github.com/mastodon/mastodon/pkgs/container/mastodon){ .card-link title=Container}

    /// success
    Follow me on the Fediverse: [@tylernguyen@tylernguyen.social](https://tylernguyen.social/@tylernguyen)
    ///

</div>

<div class="grid cards" markdown>

- ![PostgreSQL](https://assets.tylernguyen.wiki/logos/PostgreSQL.svg){ .twemoji } [PostgreSQL](https://www.postgresql.org/)
[:octicons-container-16:{ .docker }](https://hub.docker.com/_/postgres){ .card-link title=Container}

- ![Redis](https://assets.tylernguyen.wiki/logos/Redis.svg){ .twemoji } [Redis](https://redis.io/)
[:octicons-container-16:{ .docker }](https://hub.docker.com/_/redis){ .card-link title=Container}

- :simple-elasticsearch:{ .elasticsearch } [Elasticsearch](https://www.elastic.co/elasticsearch)
[:octicons-container-16:{ .docker }](https://hub.docker.com/_/elasticsearch/tags){ .card-link title=Container}

</div>

## Cloudflare Zero Trust

![Cloudflare Zero Trust](https://assets.tylernguyen.wiki/logos/Cloudflare-Zero-Trust.svg){ align=right width=125 }

I use Cloudflare Tunnel[^1] (part of the Zero Trust suite) to expose some services to the public, notably my [:simple-mastodon:{ .mastodon } Mastodon](https://tylernguyen.social/@tylernguyen) and Gitea instance.

<div class="grid cards" markdown>

- :simple-cloudflare:{ .cloudflare } [cloudflare/cloudflared](https://github.com/cloudflare/cloudflared)
[:octicons-container-16:{ .docker }](https://hub.docker.com/r/cloudflare/cloudflared){ .card-link title=Container}

</div>

[^1]: [Cloudflare Docs: How Cloudflare Tunnel Works :octicons-link-external-16:](https://developers.cloudflare.com/cloudflare-one/connections/connect-apps).

[:octicons-link-external-16: Homepage](https://www.cloudflare.com/products/zero-trust/){ .md-button }
[:fontawesome-solid-money-bill:](https://www.cloudflare.com/plans/zero-trust-services/#overview){ .card-link title=Pricing}
[:fontawesome-regular-eye:](https://www.cloudflare.com/privacypolicy/){ .card-link title="Privacy Policy" }

## Tailscale

<div class="grid cards" markdown>

- <figure markdown>
    <p align="center">
    ![Tailscale](https://assets.tylernguyen.wiki/logos/Tailscale-light.svg#only-light){ width=300 }
    ![Tailscale](https://assets.tylernguyen.wiki/logos/Tailscale-dark.svg#only-dark){ width=300 }
    </p>
    </figure>

</div>

Tailscale is my preferred remote solution for accessing the home network.

<div class="grid cards" markdown>

- ![tailscale/golink](https://assets.tylernguyen.wiki/logos/Tailscale.png){ .twemoji } [tailscale/golink](https://github.com/tailscale/golink)
[:octicons-container-16:{ .docker }](https://github.com/tailscale/golink/pkgs/container/golink){ .card-link title=Container}

- ![tailscale-dev/tclip](https://assets.tylernguyen.wiki/logos/Tailscale.png){ .twemoji } [tailscale-dev/tclip](https://github.com/tailscale-dev/tclip)
[:octicons-container-16:{ .docker }](https://github.com/tailscale-dev/tclip/pkgs/container/tclip){ .card-link title=Container}

</div>

[:octicons-link-external-16: Homepage](https://tailscale.com/){ .md-button }
[:fontawesome-solid-money-bill:](https://tailscale.com/pricing){ .card-link title=Pricing}
[:fontawesome-regular-eye:](https://tailscale.com/privacy-policy){ .card-link title="Privacy Policy" }
[:octicons-markdown-16:](https://tailscale.com/kb/1017/install?slug=kb&slug=1017&slug=install){ .card-link title=Documentation}
[:fontawesome-regular-file-code:](https://github.com/tailscale/tailscale){ .card-link title="Source Code" }
