---
icon: lucide/server
tags:
  - evergreen
  - uses
---

# Self-hosted

## Unraid

<div class="grid cards" markdown>

- <figure markdown>
    <p align="center">
    ![Unraid](https://assets.tylernguyen.wiki/logos/Unraid-light.svg#only-light){ width=250 }
    ![Unraid](https://assets.tylernguyen.wiki/logos/Unraid-dark.svg#only-dark){ width=250 }
    </p>
    </figure>

</div>

Unraid is a <span class="solarized-red">:material-lock: __proprietary__</span>, <span class="solarized-green">:lucide-circle-dollar-sign: __commercial__</span> NAS operating system.

[Homepage :octicons-arrow-up-right-16:](https://unraid.net/){ .md-button }
[:lucide-circle-dollar-sign:](https://unraid.net/pricing){ title=Pricing}
[:octicons-markdown-16:](https://wiki.unraid.net/Documentation){ title=Documentation}

Primary usage is media archival, its consumption, and sharing. The data stored is __non-personal and easily replaceable__.

Thus is the primary reason I chose :simple-unraid:{ .unraid } [Unraid :octicons-arrow-up-right-16:](https://unraid.net/) over :simple-truenas:{ .truenas } [TrueNas :octicons-arrow-up-right-16:](https://www.truenas.com/). Unraid's parity function is also better at maximizing usable storage, and dealing with mixed drive capacities.

__See [.wiki/hardware :octicons-arrow-down-left-16:](hardware.md) for server hardware specs.__

## Public Instances

<div class="grid cards" markdown>

- :simple-mastodon:{ .mastodon } [__Mastodon__: _tylernguyen.social_ :octicons-arrow-up-right-16:](https://tylernguyen.social/@tylernguyen)
[:octicons-container-16:{ .docker }](https://github.com/mastodon/mastodon/pkgs/container/mastodon){ title=Container}
[:lucide-file-code-corner:](https://github.com/mastodon/mastodon){ title="Source Code" }

</div>

<div class="grid cards" markdown>

- :simple-forgejo:{ .forgejo } [__Forgejo__: _tylernguyen.codes_ :octicons-arrow-up-right-16:](https://tylernguyen.codes/)
[:octicons-container-16:{ .docker }](https://codeberg.org/forgejo/-/packages/container/forgejo/versions){ title=Container}

</div>

<div class="grid cards" markdown>

- ![Koito](https://assets.tylernguyen.wiki/logos/Koito.webp){ .twemoji } [__Koito__: _koito.tylernguyen.app_](https://koito.tylernguyen.app)
[:octicons-container-16:{ .docker }](https://hub.docker.com/r/gabehf/koito){ title=Container}
[:lucide-file-code-corner:](https://github.com/gabehf/Koito/){ title="Source Code" }

</div>

## Home :lucide-house-wifi:

<div class="grid cards" markdown>

- :simple-homeassistant:{ .homeassistant } [Home Assistant :octicons-arrow-up-right-16:](https://www.home-assistant.io/)
[:lucide-file-code-corner:](https://github.com/home-assistant/core){ title="Source Code" }

</div>

## Network :material-server-network-outline:

<div class="grid cards" markdown>

- :simple-cloudflare:{ .cloudflare } [Cloudflare :octicons-arrow-up-right-16:](https://www.cloudflare.com/)
[:octicons-container-16:{ .docker }](https://hub.docker.com/r/cloudflare/cloudflared){ title=Container}

- ![Tailscale](https://assets.tylernguyen.wiki/logos/Tailscale.webp){ .twemoji } [Tailscale :octicons-arrow-up-right-16:](https://tailscale.com/)

- ![Pocket ID](https://assets.tylernguyen.wiki/logos/pocket-id-light.svg#only-light){ .twemoji } ![Pocket ID](https://assets.tylernguyen.wiki/logos/pocket-id-dark.svg#only-dark){ .twemoji } [Pocket ID :octicons-arrow-up-right-16:](https://pocket-id.org/)
[:octicons-container-16:{ .docker }](https://hub.docker.com/r/linuxserver/plex){ title=Container}

</div>

## Indexing :material-file-table-box-multiple-outline:

<div class="grid cards" markdown>

- ![Prowlarr](https://assets.tylernguyen.wiki/logos/prowlarr.svg){ .twemoji } [Prowlarr :octicons-arrow-up-right-16:](https://prowlarr.com/)
[:octicons-container-16:{ .docker }](https://hub.docker.com/r/linuxserver/prowlarr){ title=Container}

- ![autobrr](https://assets.tylernguyen.wiki/logos/autobrr.svg){ .twemoji } [autobrr :octicons-arrow-up-right-16:](https://github.com/autobrr/autobrr)
[:octicons-container-16:{ .docker }](https://github.com/autobrr/autobrr/pkgs/container/autobrr){ title=Container}

</div>

## Archiving :material-folder-download-outline:

<div class="grid cards" markdown>

- ![qBittorrent](https://assets.tylernguyen.wiki/logos/qbittorrent.svg){ .twemoji } [qBittorrent :octicons-arrow-up-right-16:](https://www.qbittorrent.org/)
[:octicons-container-16:{ .docker }](https://github.com/hotio/qbittorrent/pkgs/container/qbittorrent){ title=Container}

- ![qui](https://assets.tylernguyen.wiki/logos/autobrr.svg){ .twemoji } [qui :octicons-arrow-up-right-16:](https://github.com/autobrr/qui)
[:octicons-container-16:{ .docker }](https://github.com/autobrr/qui/pkgs/container/qui){ title=Container}

- ![SABnzbd](https://assets.tylernguyen.wiki/logos/sabnzbd-light.svg#only-light){ .twemoji } ![SABnzbd](https://assets.tylernguyen.wiki/logos/sabnzbd-dark.svg#only-dark){ .twemoji } [SABnzbd:octicons-arrow-up-right-16:](https://sabnzbd.org/)
[:octicons-container-16:{ .docker }](https://hub.docker.com/r/linuxserver/sabnzbd){ title=Container}

- ![rmcrackan/Libation](https://assets.tylernguyen.wiki/logos/Libation.svg){ .twemoji } [rmcrackan/Libation :octicons-arrow-up-right-16:](https://github.com/rmcrackan/Libation)
[:octicons-container-16:{ .docker }](https://hub.docker.com/r/rmcrackan/libation/tags){ title=Container}
[:lucide-file-code-corner:](https://github.com/rmcrackan/Libation){ title="Source Code" }

</div>

I prefer Hotio's image for ![qBittorrent](https://assets.tylernguyen.wiki/logos/qbittorrent.svg){ .twemoji } qBittorrent as :simple-protonvpn:{ .protonvpn } ProtonVPN support is built-in. Otherwise, the process for port forwarding through a VPN can be bothersome [^1].

I never interface with ![qBittorrent](https://assets.tylernguyen.wiki/logos/qbittorrent.svg){ .twemoji } qBittorrent through the stock WebUI. Instead, I use ![autobrr/qui](https://assets.tylernguyen.wiki/logos/autobrr.svg){ .twemoji } qui for everything.

[^1]: [ProtonVPN: How to manually set up port forwarding :octicons-arrow-up-right-16:](https://protonvpn.com/support/port-forwarding-manual-setup).

## Media :material-multimedia:

<div class="grid cards" markdown>

- ![plex](https://assets.tylernguyen.wiki/logos/plex.svg){ .twemoji } [Plex Media Server :octicons-arrow-up-right-16:](https://www.plex.tv/)
[:octicons-container-16:{ .docker }](https://hub.docker.com/r/linuxserver/plex){ title=Container}

- ![Audiobookshelf](https://assets.tylernguyen.wiki/logos/audiobookshelf.svg){ .twemoji } [Audiobookshelf :octicons-arrow-up-right-16:](https://www.audiobookshelf.org/)
[:octicons-container-16:{ .docker }](https://github.com/advplyr/audiobookshelf/pkgs/container/audiobookshelf){ title=Container}
[:lucide-file-code-corner:](https://github.com/advplyr/audiobookshelf){ title="Source Code" }

- ![Kavita](https://assets.tylernguyen.wiki/logos/kavita.svg){ .twemoji } [Kavita :octicons-arrow-up-right-16:](https://www.kavitareader.com/)
[:octicons-container-16:{ .docker }](https://hub.docker.com/r/linuxserver/kavita){ title=Container}
[:lucide-file-code-corner:](https://github.com/Kareadita/Kavita){ title="Source Code" }

- :simple-freshrss:{ .freshrss } [FreshRSS :octicons-arrow-up-right-16:](https://freshrss.org/)
[:octicons-container-16:{ .docker }](https://hub.docker.com/r/linuxserver/freshrss){ title=Container}
[:lucide-file-code-corner:](https://github.com/FreshRSS/FreshRSS){ title="Source Code" }

</div>

### Media Management :lucide-tag:

<div class="grid cards" markdown>

- :simple-sonarr:{ .sonarr } [Sonarr :octicons-arrow-up-right-16:](https://sonarr.tv/)
[:octicons-container-16:{ .docker }](https://hub.docker.com/r/linuxserver/sonarr){ title=Container}

- :simple-radarr:{ .radarr } [Radarr :octicons-arrow-up-right-16:](https://radarr.video/)
[:octicons-container-16:{ .docker }](https://hub.docker.com/r/linuxserver/radarr){ title=Container}

- ![Calibre](https://assets.tylernguyen.wiki/logos/calibre.svg){ .twemoji } [Calibre :octicons-arrow-up-right-16:](https://calibre-ebook.com/)
[:octicons-container-16:{ .docker }](https://hub.docker.com/r/linuxserver/calibre){ title=Container}

- ![Kometa](https://assets.tylernguyen.wiki/logos/Kometa.svg){ .twemoji } [Kometa :octicons-arrow-up-right-16:](https://github.com/meisnate12/Plex-Meta-Manager)
[:octicons-container-16:{ .docker }](https://hub.docker.com/r/kometateam/kometa){ title=Container}
[:lucide-file-code-corner:](https://github.com/Kometa-Team/Kometa){ title="Source Code" }

- ![Kometa/ImageMaid](https://assets.tylernguyen.wiki/logos/Kometa.svg){ .twemoji } [Kometa/ImageMaid :octicons-arrow-up-right-16:](https://github.com/meisnate12/Plex-Meta-Manager)
[:octicons-container-16:{ .docker }](https://hub.docker.com/r/kometateam/imagemaid){ title=Container}

</div>

### Media Scrobblers :lucide-rss:

<div class="grid cards" markdown>

- ![plexanibridge](https://assets.tylernguyen.wiki/logos/plexanibridge.svg){ .twemoji } [PlexAniBridge :octicons-arrow-up-right-16:](https://github.com/eliasbenb/PlexAniBridge)
[:octicons-container-16:{ .docker }](https://github.com/eliasbenb/PlexAniBridge/pkgs/container/plexanibridge){ title=Container}

- ![FoxxMD/multi-scrobbler](https://assets.tylernguyen.wiki/logos/Multi-scrobbler.svg){ .twemoji } [FoxxMD/multi-scrobbler :octicons-arrow-up-right-16:](https://github.com/foxxmd/multi-scrobbler)
[:octicons-container-16:{ .docker }](https://github.com/FoxxMD/multi-scrobbler/pkgs/container/multi-scrobbler){ title=Container}

- ![Koito](https://assets.tylernguyen.wiki/logos/Koito.webp){ .twemoji } [Koito :octicons-arrow-up-right-16:](https://github.com/gabehf/koito)
[:octicons-container-16:{ .docker }](https://hub.docker.com/r/gabehf/koito){ title=Container}

</div>

## Utilities :lucide-pocket-knife:

<div class="grid cards" markdown>

- :simple-syncthing:{ .syncthing } [Syncthing :octicons-arrow-up-right-16:](https://syncthing.net/)
[:octicons-container-16:{ .docker }](https://github.com/linuxserver/docker-syncthing/pkgs/container/syncthing){ title=Container}
[:lucide-file-code-corner:](https://github.com/syncthing/syncthing){ title="Source Code" }

- ![tailscale/golink](https://assets.tylernguyen.wiki/logos/Tailscale.webp){ .twemoji } [tailscale/golink :octicons-arrow-up-right-16:](https://github.com/tailscale/golink)
[:octicons-container-16:{ .docker }](https://github.com/tailscale/golink/pkgs/container/golink){ title=Container}

- ![taildrive](https://assets.tylernguyen.wiki/logos/Tailscale.webp){ .twemoji } [taildrive :octicons-arrow-up-right-16:](https://tailscale.com/kb/1369/taildrive)

</div>

## Databases :lucide-database:

<div class="grid cards" markdown>

- ![SQLite](https://assets.tylernguyen.wiki/logos/SQLite.svg){ .twemoji } [SQLite :octicons-arrow-up-right-16:](https://sqlite.org/)

- ![PostgreSQL](https://assets.tylernguyen.wiki/logos/PostgreSQL.svg){ .twemoji } [PostgreSQL :octicons-arrow-up-right-16:](https://www.postgresql.org/)

- ![Redis](https://assets.tylernguyen.wiki/logos/Redis.svg){ .twemoji } [Redis :octicons-arrow-up-right-16:](https://redis.io/)

- :simple-elasticsearch:{ .elasticsearch } [Elasticsearch :octicons-arrow-up-right-16:](https://www.elastic.co/elasticsearch)

</div>

Whenever possible, I much prefer ![SQLite](https://assets.tylernguyen.wiki/logos/SQLite.svg){ .twemoji } [SQLite :octicons-arrow-up-right-16:](https://sqlite.org/) over ![PostgreSQL](https://assets.tylernguyen.wiki/logos/PostgreSQL.svg){ .twemoji } PostgreSQL.
