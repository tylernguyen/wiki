---
icon: lucide/book-marked
tags:
  - evergreen
  - workflow
---

# Read

## Books

<div class="grid cards" markdown>

- ![Calibre](https://assets.tylernguyen.wiki/logos/calibre.svg){ .twemoji } [Calibre :octicons-arrow-up-right-16:](https://calibre-ebook.com/)
[:lucide-container:](https://hub.docker.com/r/linuxserver/calibre){ .card-link title=Container}
- ![Kavita](https://assets.tylernguyen.wiki/logos/kavita.svg){ .twemoji } [Kavita :octicons-arrow-up-right-16:](https://www.kavitareader.com/)
[:lucide-container:](https://hub.docker.com/r/linuxserver/kavita){ .card-link title=Container}
[:fontawesome-regular-file-code:](https://github.com/Kareadita/Kavita){ .card-link title="Source Code" }
- :simple-koreader:{ .koreader } [KOReader :octicons-arrow-up-right-16:](https://github.com/koreader/koreader)

</div>

### ![Calibre](https://assets.tylernguyen.wiki/logos/calibre.svg){ .twemoji } [Calibre :octicons-arrow-up-right-16:](https://calibre-ebook.com/)

<div align="center">

```mermaid
graph LR
  standardebooks.org -- Yes --> READY
  standardebooks.org -- No --> n1["Update Metadata <br> Update Cover <br/> Polish"]
  n1 --> QC
  QC -- Pass --> READY
  QC -- Fail --> n2["Manual Edits"]
  n2 --> READY
```

</div>

/// extension | Plugins
- [janlarres/apple-books-covers :octicons-arrow-up-right-16:](https://github.com/janlarres/apple-books-covers)
- [Hardcover by RobBrazier :octicons-arrow-up-right-16:](https://github.com/RobBrazier/calibre-plugins/tree/main/plugins/hardcover)
- [NotSimone/Kobo-Metadata :octicons-arrow-up-right-16:](https://github.com/NotSimone/Kobo-Metadata)
- [jbhul/Audiobookshelf-calibre-plugin :octicons-arrow-up-right-16:](https://github.com/jbhul/Audiobookshelf-calibre-plugin)
- [harmtemolder/koreader-calibre-plugin :octicons-arrow-up-right-16:](https://github.com/harmtemolder/koreader-calibre-plugin)

///

/// setting | Settings
- Save template: `{series:'re(ifempty($,field('title')),':',' -')'}/{series:'re(ifempty($,field('title')),':',' -')'}{series_index:0>2s| - |}`
- Polish books:
    - [x] Smarten punctuation
    - [x] Update medata in the book files
    - [x] Update the cover in the book files
    - [x] Losslessly compress images
    - [x] Download external resources
    - [x] Add soft hyphens
    - [x] Upgrade book internals
///

### :simple-koreader:{ .koreader } [KOReader :octicons-arrow-up-right-16:](https://github.com/koreader/koreader)

KOReader is an <span class="solarized-orange">:lucide-folder-git-2: __open source__</span> and extensible reader for e-ink devices.

Aside from my computer, I mostly read eBooks on my [__Kobo Clara BW__](https://us.kobobooks.com/products/kobo-clara-bw).

See :simple-refinedgithub:{ .foreground } KOReader: [Installation on Kobo devices :octicons-arrow-up-right-16:](https://github.com/koreader/koreader/wiki/Installation-on-Kobo-devices).

KOReader is __VERY__ customizable and integrates well with Calibre. Anecdotally, I also think it handles ebook formats, especially `.epub`, better than other viewer software.

/// extension | Plugins and Patches
- [hardcoverapp.koplugin :octicons-arrow-up-right-16:](https://github.com/Billiam/hardcoverapp.koplugin) to scrobble reading records to ![Hardcover](https://assets.tylernguyen.wiki/logos/Hardcover.svg){ .twemoji } Hardcover.
///

/// setting | Settings
- [Bookerly :octicons-arrow-up-right-16:](https://developer.amazon.com/en-US/alexa/branding/echo-guidelines/identity-guidelines/typography) as the default reading font.
- [Berkeley Mono :octicons-arrow-up-right-16:](https://usgraphics.com/products/berkeley-mono) as the UI font.
///

## Audiobooks

/// question | [IS AUDIOBOOK READING? :octicons-arrow-up-right-16:](https://www.google.com/search?q=is+audiobook+reading)
:lucide-check-check:{ .solarized-green } __Yes__, how else would blind people `read` ?
///

<div class="grid cards" markdown>

- ![rmcrackan/Libation](https://assets.tylernguyen.wiki/logos/Libation.svg){ .twemoji } [Libation :octicons-arrow-up-right-16:](https://github.com/rmcrackan/Libation)
[:lucide-container:](https://hub.docker.com/r/rmcrackan/libation/tags){ title=Container}
[:lucide-file-code-corner:](https://github.com/rmcrackan/Libation){ title="Source Code" }
- ![Audiobookshelf](https://assets.tylernguyen.wiki/logos/audiobookshelf.svg){ .twemoji } [Audiobookshelf :octicons-arrow-up-right-16:](https://www.audiobookshelf.org/)
[:lucide-container:](https://github.com/advplyr/audiobookshelf/pkgs/container/audiobookshelf){ .card-link title=Container}
[:fontawesome-regular-file-code:](https://github.com/advplyr/audiobookshelf){ .card-link title="Source Code" }
- ![Prologue](https://assets.tylernguyen.wiki/logos/Prologue.webp){ .twemoji } [Prologue (iOS) :octicons-arrow-up-right-16:](https://apps.apple.com/us/app/prologue-audiobook-player/id1459223267)

</div>

<div align="center">

```mermaid
graph LR
  Audible --> Libation
  Libation --> Audiobookshelf
  other --> Audiobookshelf
  Audiobookshelf --> n1["Prologue (iOS)"]
  Audiobookshelf --> n2["Built-in PWA"]
```

</div>

- Audiobooks from :simple-audible:{ .audible } Audible are archived in `.m4b` using ![rmcrackan/Libation](https://assets.tylernguyen.wiki/logos/Libation.svg){ .twemoji } Libation.
- DRM-free audiobook files are manually renamed and organized. I haven't figured out an automation workflow for this yet.

```json title="Libation - Settings.json"
{
  "FolderTemplate": "<first author>/ <title short> (<year>) [<id>]",
  "FileTemplate": "<title> (<year>) [<id>]"
}
```

- `[<id>]` is the :simple-audible:{ .audible } Audible book ID, ASIN.

This is what the audiobooks dir looks like.

```Ruby
audiobooks/
├─ Viet Thanh Nguyen/
│  ├─ The Sympathizer (2014) [B00W1Y6MOQ]/
│  │  ├─ The Sympathizer (2014) [B00W1Y6MOQ].m4b
│  │  ├─ cover.jpg
│  │  ├─ metadata.json
│  │  ├─ metadata.abs
│  ├─ The Committed (2021) [B08SYKJP69]/
├─ Chang-Rae Lee/
├─ David Grann/
├─ .../
```

- ![Audiobookshelf](https://assets.tylernguyen.wiki/logos/audiobookshelf.svg){ .twemoji } Audiobookshelf manages `cover.jpg`, `metadata.json`, `metadata.abs`.
- Preferred format is `.m4b`, strictly 1 file per book.
