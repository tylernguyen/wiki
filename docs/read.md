---
icon: lucide/book-marked
tags:
  - evergreen
  - workflow
---

# Read

> [!question] [IS AUDIOBOOK READING? :lucide-arrow-up-right:](https://www.google.com/search?q=is+audiobook+reading)
> :lucide-check-check:{ .solarized-green } __Yes__, how else would blind people `read` ?

## Calibre

- ![Calibre](https://assets.tylernguyen.wiki/logos/calibre.svg){ .twemoji } [Calibre :lucide-arrow-down-left:](#calibre)

Watches `/data/media/import/books/`, and imports to `/data/media/books/`.

> [!extension]- Plugins
> - [janlarres/apple-books-covers :lucide-arrow-up-right:](https://github.com/janlarres/apple-books-covers)
> - [Hardcover by RobBrazier :lucide-arrow-up-right:](https://github.com/RobBrazier/calibre-plugins/tree/main/plugins/hardcover)
> - [NotSimone/Kobo-Metadata :lucide-arrow-up-right:](https://github.com/NotSimone/Kobo-Metadata)
> - [jbhul/Audiobookshelf-calibre-plugin :lucide-arrow-up-right:](https://github.com/jbhul/Audiobookshelf-calibre-plugin)
> - [harmtemolder/koreader-calibre-plugin :lucide-arrow-up-right:](https://github.com/harmtemolder/koreader-calibre-plugin)

> [!setting]- Settings
> - Save template: `{series:'re(ifempty($,field('title')),':',' -')'}/{series:'re(ifempty($,field('title')),':',' -')'}{series_index:0>2s| - |}`
> - Polish books:
>     - [x] Smarten punctuation
>     - [x] Update medata in the book files
>     - [x] Update the cover in the book files
>     - [x] Losslessly compress images
>     - [x] Download external resources
>     - [x] Add soft hyphens
>     - [x] Upgrade book internals

## Kavita

- ![Kavita](https://assets.tylernguyen.wiki/logos/kavita.svg){ .twemoji } [Kavita :lucide-arrow-up-right:](https://www.kavitareader.com/)
  [:lucide-container:](https://hub.docker.com/r/linuxserver/kavita){ .extra title=Container}
  [:lucide-file-code-corner:](https://github.com/Kareadita/Kavita){ .extra title="Source Code" }

Reads `/data/media/books/`, serve using PWA.

## KOReader

- :simple-koreader:{ .koreader } [KOReader :lucide-arrow-up-right:](https://github.com/koreader/koreader) on my [Kobo Clara BW :lucide-arrow-up-right:](https://us.kobobooks.com/products/kobo-clara-bw).

> [!extension]- Plugins and Patches
> - [hardcoverapp.koplugin :lucide-arrow-up-right:](https://github.com/Billiam/hardcoverapp.koplugin) to scrobble reading records to ![Hardcover](https://assets.tylernguyen.wiki/logos/Hardcover.svg){ .twemoji } Hardcover.

> [!setting]- Settings
> - [Bookerly :lucide-arrow-up-right:](https://developer.amazon.com/en-US/alexa/branding/echo-guidelines/identity-guidelines/typography) as the default reading font.
> - [Berkeley Mono :lucide-arrow-up-right:](https://usgraphics.com/products/berkeley-mono) as the UI font.

## Libation

- ![rmcrackan/Libation](https://assets.tylernguyen.wiki/logos/Libation.svg){ .twemoji } [Libation :lucide-arrow-up-right:](https://github.com/rmcrackan/Libation)
  [:lucide-container:](https://hub.docker.com/r/rmcrackan/libation/tags){ .extra title=Container}
  [:lucide-file-code-corner:](https://github.com/rmcrackan/Libation){ .extra title="Source Code" }

```json title="Settings.json"
{
  "FolderTemplate": "<first author>/ <title short> (<year>) [<id>]",
  "FileTemplate": "<title> (<year>) [<id>]"
}
```

Where `[<id>]` is the Amazon Standard Identification Number (ASIN).

## Audiobookshelf

- ![Audiobookshelf](https://assets.tylernguyen.wiki/logos/audiobookshelf.svg){ .twemoji } [Audiobookshelf :lucide-arrow-up-right:](https://www.audiobookshelf.org/)
  [:lucide-container:](https://github.com/advplyr/audiobookshelf/pkgs/container/audiobookshelf){ .extra title=Container}
  [:lucide-file-code-corner:](https://github.com/advplyr/audiobookshelf){ .extra title="Source Code" }

Reads `/data/media/audiobooks`

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

Where `cover.jpg`, `metadata.json`, `metadata.abs` are generated/managed by Audiobookshelf.

## Prologue

- ![Prologue](https://assets.tylernguyen.wiki/logos/Prologue.webp){ .twemoji } [Prologue (iOS) :lucide-arrow-up-right:](https://apps.apple.com/us/app/prologue-audiobook-player/id1459223267)

The built-in Audiobookshelf PWA is adequate on mobile. But Prologue is my preferred client on iOS.
