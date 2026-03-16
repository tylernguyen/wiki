---
icon: lucide/server
tags:
  - evergreen
  - uses
---

# Self-hosted

<div class="grid cards" markdown>

- ### :simple-unraid:{ .unraid } [Unraid :lucide-arrow-up-right:](https://unraid.net)

    My primary usage is media archival, its consumption, and sharing. The data stored is __non-personal and easily replaceable__.

    Hence the reason I chose :simple-unraid:{ .unraid } [Unraid :lucide-arrow-up-right:](https://unraid.net/) over :simple-truenas:{ .truenas } [TrueNas :lucide-arrow-up-right:](https://www.truenas.com/). Unraid's parity function is also better at maximizing usable storage, and dealing with mixed drive capacities.

</div>

__See [/hardware#server :lucide-arrow-down-left:](hardware.md#server) for hardware specs.__

## Public

- :simple-mastodon:{ .mastodon } __Mastodon__: [_tylernguyen.social_ :lucide-arrow-up-right:](https://tylernguyen.social/@tylernguyen)
  [:lucide-container:](https://github.com/mastodon/mastodon/pkgs/container/mastodon){ .extra title=Container}
  [:lucide-file-code-corner:](https://github.com/mastodon/mastodon){ .extra title="Source Code" }

I mostly lurk and read on Mastodon. But I do intend post more in the future. My favorite client for both web and iOS is ![Phanpy](https://assets.tylernguyen.wiki/logos/Phanpy.svg){ .twemoji } [Phanpy :lucide-arrow-up-right:](https://phanpy.social/).

- :simple-forgejo:{ .forgejo } __Forgejo__: [_tylernguyen.codes_ :lucide-arrow-up-right:](https://tylernguyen.codes/)
  [:lucide-container:](https://codeberg.org/forgejo/-/packages/container/forgejo/versions){ .extra title=Container}
- ![Koito](https://assets.tylernguyen.wiki/logos/Koito.webp){ .twemoji } __Koito__: [_koito.tylernguyen.app_](https://koito.tylernguyen.app)
  [:lucide-container:](https://hub.docker.com/r/gabehf/koito){ .extra title=Container}
  [:lucide-file-code-corner:](https://github.com/gabehf/Koito/){ .extra title="Source Code" }

## Home

- :simple-homeassistant:{ .homeassistant } [Home Assistant :lucide-arrow-up-right:](https://www.home-assistant.io/)
  [:lucide-file-code-corner:](https://github.com/home-assistant/core){ .extra title="Source Code" }

I'm not too big into home automation. But Home Assistant has been set and forget for the few IoT devices I do have, which is nice.

## Network

- :simple-cloudflare:{ .cloudflare } [Cloudflare Tunnel :lucide-arrow-up-right:](https://www.cloudflare.com/)
  [:lucide-container:](https://hub.docker.com/r/cloudflare/cloudflared){ .extra title=Container}
- ![Tailscale](https://assets.tylernguyen.wiki/logos/Tailscale.webp){ .twemoji } [Tailscale :lucide-arrow-up-right:](https://tailscale.com/)
- ![Pocket ID](https://assets.tylernguyen.wiki/logos/pocket-id-light.svg#only-light){ .twemoji } ![Pocket ID](https://assets.tylernguyen.wiki/logos/pocket-id-dark.svg#only-dark){ .twemoji } [Pocket ID :lucide-arrow-up-right:](https://pocket-id.org/)
  [:lucide-container:](https://github.com/pocket-id/pocket-id/pkgs/container/pocket-id){ .extra title=Container}

## Indexing

- ![Prowlarr](https://assets.tylernguyen.wiki/logos/prowlarr.svg){ .twemoji } [Prowlarr :lucide-arrow-up-right:](https://prowlarr.com/)
  [:lucide-container:](https://hub.docker.com/r/linuxserver/prowlarr){ .extra title=Container}
- ![autobrr](https://assets.tylernguyen.wiki/logos/autobrr.svg){ .twemoji } [autobrr :lucide-arrow-up-right:](https://github.com/autobrr/autobrr)
  [:lucide-container:](https://github.com/autobrr/autobrr/pkgs/container/autobrr){ .extra title=Container}

## Archiving

- ![qBittorrent](https://assets.tylernguyen.wiki/logos/qbittorrent.svg){ .twemoji } [qBittorrent :lucide-arrow-up-right:](https://www.qbittorrent.org/)
  [:lucide-container:](https://github.com/hotio/qbittorrent/pkgs/container/qbittorrent){ .extra title=Container}

I prefer Hotio's Docker image as :simple-protonvpn:{ .protonvpn } ProtonVPN support is built-in. Otherwise, port forwarding for ProtonVPN can be troublesome[^1].

[^1]: [ProtonVPN: How to manually set up port forwarding :lucide-arrow-up-right:](https://protonvpn.com/support/port-forwarding-manual-setup).
- ![qui](https://assets.tylernguyen.wiki/logos/autobrr.svg){ .twemoji } [qui :lucide-arrow-up-right:](https://github.com/autobrr/qui)
  [:lucide-container:](https://github.com/autobrr/qui/pkgs/container/qui){ .extra title=Container}

I never interface with ![qBittorrent](https://assets.tylernguyen.wiki/logos/qbittorrent.svg){ .twemoji } qBittorrent through the stock WebUI.

- ![SABnzbd](https://assets.tylernguyen.wiki/logos/sabnzbd-light.svg#only-light){ .twemoji } ![SABnzbd](https://assets.tylernguyen.wiki/logos/sabnzbd-dark.svg#only-dark){ .twemoji } [SABnzbd :lucide-arrow-up-right:](https://sabnzbd.org/)
  [:lucide-container:](https://hub.docker.com/r/linuxserver/sabnzbd){ .extra title=Container}
- ![Libation](https://assets.tylernguyen.wiki/logos/Libation.svg){ .twemoji } [Libation :lucide-arrow-up-right:](https://getlibation.com/)
  [:lucide-container:](https://hub.docker.com/r/rmcrackan/libation/tags){ .extra title=Container}
  [:lucide-file-code-corner:](https://github.com/rmcrackan/Libation){ .extra title="Source Code" }

## Media

- ![plex](https://assets.tylernguyen.wiki/logos/plex.svg){ .twemoji } [Plex Media Server :lucide-arrow-up-right:](https://www.plex.tv/)
  [:lucide-container:](https://hub.docker.com/r/linuxserver/plex){ .extra title=Container}
- ![Audiobookshelf](https://assets.tylernguyen.wiki/logos/audiobookshelf.svg){ .twemoji } [Audiobookshelf :lucide-arrow-up-right:](https://www.audiobookshelf.org/)
  [:lucide-container:](https://github.com/advplyr/audiobookshelf/pkgs/container/audiobookshelf){ .extra title=Container}
  [:lucide-file-code-corner:](https://github.com/advplyr/audiobookshelf){ .extra title="Source Code" }
- ![Kavita](https://assets.tylernguyen.wiki/logos/kavita.svg){ .twemoji } [Kavita :lucide-arrow-up-right:](https://www.kavitareader.com/)
  [:lucide-container:](https://hub.docker.com/r/linuxserver/kavita){ .extra title=Container}
  [:lucide-file-code-corner:](https://github.com/Kareadita/Kavita){ .extra title="Source Code" }
- :simple-freshrss:{ .freshrss } [FreshRSS :lucide-arrow-up-right:](https://freshrss.org/)
  [:lucide-container:](https://hub.docker.com/r/linuxserver/freshrss){ .extra title=Container}
  [:lucide-file-code-corner:](https://github.com/FreshRSS/FreshRSS){ .extra title="Source Code" }

### Media Management

- :simple-sonarr:{ .sonarr } [Sonarr :lucide-arrow-up-right:](https://sonarr.tv/)
  [:lucide-container:](https://hub.docker.com/r/linuxserver/sonarr){ .extra title=Container}
- :simple-radarr:{ .radarr } [Radarr :lucide-arrow-up-right:](https://radarr.video/)
  [:lucide-container:](https://hub.docker.com/r/linuxserver/radarr){ .extra title=Container}
- ![Calibre](https://assets.tylernguyen.wiki/logos/calibre.svg){ .twemoji } [Calibre :lucide-arrow-up-right:](https://calibre-ebook.com/)
  [:lucide-container:](https://hub.docker.com/r/linuxserver/calibre){ .extra title=Container}
- ![Kometa](https://assets.tylernguyen.wiki/logos/Kometa.svg){ .twemoji } [Kometa :lucide-arrow-up-right:](https://github.com/meisnate12/Plex-Meta-Manager)
  [:lucide-container:](https://hub.docker.com/r/kometateam/kometa){ .extra title=Container}
  [:lucide-file-code-corner:](https://github.com/Kometa-Team/Kometa){ .extra title="Source Code" }
- ![Kometa/ImageMaid](https://assets.tylernguyen.wiki/logos/Kometa.svg){ .twemoji } [Kometa/ImageMaid :lucide-arrow-up-right:](https://github.com/meisnate12/Plex-Meta-Manager)
  [:lucide-container:](https://hub.docker.com/r/kometateam/imagemaid){ .extra title=Container}

### Media Scrobblers

- ![anibridge](https://assets.tylernguyen.wiki/logos/plexanibridge.svg){ .twemoji } [AniBridge :lucide-arrow-up-right:](https://github.com/anibridge/anibridge)
  [:lucide-container:](https://github.com/anibridge/anibridge/pkgs/container/anibridge){ .extra title=Container}
- ![FoxxMD/multi-scrobbler](https://assets.tylernguyen.wiki/logos/Multi-scrobbler.svg){ .twemoji } [FoxxMD/multi-scrobbler :lucide-arrow-up-right:](https://github.com/foxxmd/multi-scrobbler)
  [:lucide-container:](https://github.com/FoxxMD/multi-scrobbler/pkgs/container/multi-scrobbler){ .extra title=Container}
- ![Koito](https://assets.tylernguyen.wiki/logos/Koito.webp){ .twemoji } [Koito :lucide-arrow-up-right:](https://github.com/gabehf/koito)
  [:lucide-container:](https://hub.docker.com/r/gabehf/koito){ .extra title=Container}

## Utilities

- :simple-syncthing:{ .syncthing } [Syncthing :lucide-arrow-up-right:](https://syncthing.net/)
  [:lucide-container:](https://github.com/linuxserver/docker-syncthing/pkgs/container/syncthing){ .extra title=Container}
  [:lucide-file-code-corner:](https://github.com/syncthing/syncthing){ .extra title="Source Code" }
- ![tailscale/golink](https://assets.tylernguyen.wiki/logos/Tailscale.webp){ .twemoji } [tailscale/golink :lucide-arrow-up-right:](https://github.com/tailscale/golink)
  [:lucide-container:](https://github.com/tailscale/golink/pkgs/container/golink){ .extra title=Container}
- ![taildrive](https://assets.tylernguyen.wiki/logos/Tailscale.webp){ .twemoji } [taildrive :lucide-arrow-up-right:](https://tailscale.com/kb/1369/taildrive)

## Databases

- ![SQLite](https://assets.tylernguyen.wiki/logos/SQLite.svg){ .twemoji } [SQLite :lucide-arrow-up-right:](https://sqlite.org/)
- ![PostgreSQL](https://assets.tylernguyen.wiki/logos/PostgreSQL.svg){ .twemoji } [PostgreSQL :lucide-arrow-up-right:](https://www.postgresql.org/)
- ![Redis](https://assets.tylernguyen.wiki/logos/Redis.svg){ .twemoji } [Redis :lucide-arrow-up-right:](https://redis.io/)
- :simple-elasticsearch:{ .elasticsearch } [Elasticsearch :lucide-arrow-up-right:](https://www.elastic.co/elasticsearch)

Whenever possible, I much prefer ![SQLite](https://assets.tylernguyen.wiki/logos/SQLite.svg){ .twemoji } [SQLite :lucide-arrow-up-right:](https://sqlite.org/) over ![PostgreSQL](https://assets.tylernguyen.wiki/logos/PostgreSQL.svg){ .twemoji } PostgreSQL.
