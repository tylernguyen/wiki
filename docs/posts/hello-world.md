# Hello, World!

Building a knowledge base and maintaining a blog has always been something I've always wanted to do. So after an extended period of on and off development, I'm now proud to say that my personal wiki is now public. The following is a quick overview of the stack used in creating this website.

<!-- more -->

## Markdown :octicons-markdown-16:

[Markdown](https://en.wikipedia.org/wiki/Markdown) is the de-facto markup language. The standard is open, simple, and widely supported. Files written in Markdown are human-readable without a WYSIWYG editor. So I see no particular reasons to use anything else.

Markdown, however, is conservative in its syntax, features, and specifications. Implementations(flavors) of Markdown would take advantage its barebone-design to add components, integrations, and features.

Having used several different interations in Markdown, I still don't have a strong preference for any particular implementation. So I paid no mind to the choices of Markdown flavors, and would be okay with whichever is defaulted to by the website framework.

## Static Site Generator

Creating a website with React, Javascript, MDX, and Tailwind CSS all sounded like a very fun project to me in the beginning. But maintaining said infrastructure seems rather involved and time-consuming for a personal wiki. I wanted a place to organize my brain, and the last thing I want to deal with is JavaScript dependencies breaking.

<div class="grid cards" markdown>

- :simple-materialformkdocs:{ .materialformkdocs } [Material for MkDocs :octicons-arrow-up-right-16:](https://squidfunk.github.io/mkdocs-material/) [_Insiders_](https://squidfunk.github.io/mkdocs-material/insiders/)
[:fontawesome-regular-file-code:](https://github.com/squidfunk/mkdocs-material){ .card-link title="Source Code" }
[:octicons-law-16:](https://github.com/squidfunk/mkdocs-material/blob/master/LICENSE){ .card-link title=License }

</div>

Enters Material for MkDocs, the project started as a theme for the [MkDocs](https://www.mkdocs.org/) framework, but grew popular and became a framework of its own. It uses Python Markdown, which is more limited in its extensibility than something like [MDX](https://mdxjs.com/) with JavaScript.

Since I have no specific needs for MDX and other JavaScript elements anyway, I'm content with starting on Material for MkDocs. The extensions and customizations that it does have are more than enough for my intended purpose. And for starting out, the framework is robust and matured enough that I can focus more on writing and less time on building the website.

<div class="grid cards" markdown>

- :simple-docker:{ .docker } [Docker Desktop :octicons-arrow-up-right-16:](https://www.docker.com/products/docker-desktop/)
[:fontawesome-solid-money-bill:](https://www.docker.com/pricing/){ .card-link title="Pricing" }
- ![OrbStack](https://assets.tylernguyen.wiki/logos/OrbStack.webp){ .twemoji } [OrbStack :octicons-arrow-up-right-16:](https://orbstack.dev/)
[:fontawesome-solid-money-bill:](https://orbstack.dev/pricing){ .card-link title="Pricing" }

</div>

The site is built locally for previewing with a Docker image of Material for MkDocs Insiders.

## Cloudflare Stack :simple-cloudflare:{ .cloudflare }

<div class="grid cards" markdown>

- :simple-cloudflare:{ .cloudflare } [Cloudflare Domain Registar :octicons-arrow-up-right-16:](https://www.cloudflare.com/products/registrar/)
- :simple-cloudflare:{ .cloudflare } [Cloudflare DNS :octicons-arrow-up-right-16:](https://www.cloudflare.com/)
- :simple-cloudflare:{ .cloudflare } [Cloudflare R2 :octicons-arrow-up-right-16:](https://www.cloudflare.com/products/r2/)
- :simple-cloudflarepages:{ .cloudflarepages } [Cloudflare Pages :octicons-arrow-up-right-16:](https://pages.cloudflare.com/)

</div>

As a passion project, I wanted to limit costs as much as possible. Cloudflare Domain Registar offers [at-cost pricing :octicons-arrow-up-right-16:](https://www.cloudflare.com/products/registrar/), and the free tiers on R2 and Pages are more than enough for starting out.

Importantly, since Cloudflare basically powers the entire internet nowadays, I don't think there is a more reliable party for hosting.

## Analytics

I want to use analytics as a form of automated feedbacks, __NOT__ as a tool to create better advertisements and convert higher ROI.

Google Analytics was designed for the latter purpose, not the mention being a privacy-invasive product. It's something I block in every browser, ad-block extension, and DNS-blocker. So the thought of using it myself feels hypocritical.

I briefly considered [Plausible Analytics :octicons-arrow-up-right-16:](https://plausible.io/), but the analytics data it gives is not something that I find actionable nor particularly useful. The same issue arises with Cloudflare's built in web analytics.

<div class="grid cards" markdown>

- <figure markdown>
    <p align="center">
    ![PostHog](https://assets.tylernguyen.wiki/logos/PostHog-light.svg#only-light){ loading-lazy width=350 }
    ![PostHog](https://assets.tylernguyen.wiki/logos/PostHog-dark.svg#only-dark){ loading-lazy width=350 }
    </p>
    </figure>

</div>

Enters PostHog, which seems perfect for what I want analytics to do. Aside from the standard [web analytics :octicons-arrow-up-right-16:](https://posthog.com/web-analytics) tookit, PostHog's [session replay :octicons-arrow-up-right-16:](https://posthog.com/session-replay) seems like the perfect non-interactive feedback that I was looking for.
