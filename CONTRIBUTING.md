# How to help

Waypack's code lives in a private repository, so there are no pull requests to send here. What this
repository is for is **telling the author what is broken and what is missing** — which, for an app
built by one person, is the part that changes it fastest.

## Before you open an issue

**Please don't paste your trips.** Screenshots, exported `.waypack` files and backups carry real
names, dates, places and documents. This repository is public and indexed by search engines, and
nothing in that data helps fix a bug. If a screenshot is the only way to show the problem, blur or
rename first, or make a throwaway trip that reproduces it.

Two things that always help instead:

- **The version**, from Settings → About (it looks like `Version 1.0 (build 1)`).
- **Your phone and Android version** — and say so if it runs GrapheneOS, CalyxOS or another
  de-Googled system, because that is precisely the ground this app is built for.

## Bugs

Use the [bug report](https://github.com/bymaksym/waypack/issues/new?template=bug_report.yml)
template. The single most useful line is **what you did, step by step, until it broke**. "It crashes
sometimes" cannot be chased; "it closes when I rotate the phone on the packing screen with a bag
open" can be fixed the same evening.

If something **lost data**, say so in the title. That jumps the queue over everything else.

## Ideas

Use the [feature request](https://github.com/bymaksym/waypack/issues/new?template=feature_request.yml)
template, and tell the story rather than the solution: the trip where you needed it, and what you did
instead. A described problem survives; a described feature often turns out to be the wrong shape once
someone tries to build it.

Some things are **out of scope on purpose**, and no amount of asking will move them:

- Anything that needs a server, an account or a sync — flight itineraries read from your email,
  shared live lists, cloud backup. The app has no network permission and is not going to get one.
- Ads, analytics, or a "crash reporting" SDK.
- Anything that requires Google Play Services.

Handing a trip to another person already works, offline, through the `.waypack` file.

## Questions and conversations

[Discussions](https://github.com/bymaksym/waypack/discussions) is the place for "how do I…", packing
setups worth stealing, and anything that isn't a defect.

## Translations

The app ships in English, Spanish, Russian and Ukrainian. The Russian and Ukrainian texts were not
reviewed by native speakers — that is a known, deliberate gap, not an oversight. **If a word reads
wrong to you, open an issue with the screen and the better wording.** It is one of the most useful
things anyone can send.

## Security

A vulnerability does not go in a public issue. See [SECURITY.md](SECURITY.md).
