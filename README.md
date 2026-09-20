<div align="center">

# Waypack

**A packing and trip organizer: what to bring, by day, by bag and by person.**

[Download the latest APK](https://github.com/bymaksym/waypack/releases/latest) ·
[Report a bug](https://github.com/bymaksym/waypack/issues/new?template=bug_report.yml) ·
[Leer en español](README.es.md)

</div>

---

Waypack organizes your trips and what you pack for them — by day, by bag, by person. It works
fully offline, with no account and no ads.

> This repository is the home of Waypack's **releases, bug reports and discussions**. The app's
> source code is not public (yet).

## What it does

**Packing**
- Packing lists per trip, by category, by day and by bag.
- A two-stage check — *prepared* and *in the bag* — plus *is it ready?* for the things that can sit
  packed and still be useless, like a camera with a flat battery.
- Real units (pieces, pairs, ml, g), so the liquids bag adds itself up.
- Bags inside bags: the big case stays in the car and the overnight bag comes out of it.
- People on the trip and group gear, so a party of five doesn't carry two water filters — and the
  shared bottle nobody packed doesn't stay home.

**Your gear**
- An inventory that belongs to no trip: what each thing weighs, tagged by season. It fills itself in
  as you weigh things inside a plan.
- Gear with a life of its own: first use, falls, real expiry dates, maintenance and what broke. It
  only subtracts dates — it never decides for you.
- Templates of your own, saved from any plan, plus factory ones to start from.

**For the mountains**
- Water for the route, daylight left, food and gas.
- A first-aid kit by duration and activity, and the gear each profile asks for (summer, winter,
  glacier, rock, water, bike).
- An avalanche bulletin you type in yourself, which expires on its own.
- Barometer and altimeter, with what a phone can know and what it cannot.

**The whole trip**
- Legs, places by day, and documents — your passport is yours, not a trip's, so its expiry date is
  written in one place and Waypack crosses it against the trips still to come.
- Routes: a `.gpx` or a `.kml` travels with the trip instead of sitting in a Downloads folder with
  forty other files. Route files only, up to 10 MB — for a ticket or a photo your phone's file
  manager does it better.
- Backups you choose: Google's system backup, an automatic file in a folder of your own, or nothing
  at all. Plus a manual export, with your own password, that you can hand to whoever travels with
  you.
- English, Spanish, Russian and Ukrainian, with an in-app language switch.
- Screenshot blocking, hiding from recents, and an app lock behind your phone's own credential.

## Install

**Requires Android 8.0 (API 26) or newer.** No Google Play Services needed.

- **Direct download** — grab `app-release.apk` from the
  [latest release](https://github.com/bymaksym/waypack/releases/latest) and open it.
- **[Obtainium](https://github.com/ImranR98/Obtainium)** — point it at this repository and it will
  track new versions for you. The APK's filename stays the same on purpose so that this keeps
  working.

To check your download, compare it against the `.sha256` published with each release:

```
sha256sum app-release.apk
```

## Report a bug or ask for something

- 🐞 [Bug report](https://github.com/bymaksym/waypack/issues/new?template=bug_report.yml)
- 💡 [Feature request](https://github.com/bymaksym/waypack/issues/new?template=feature_request.yml)
- 💬 [Discussions](https://github.com/bymaksym/waypack/discussions) — questions, packing setups,
  anything that isn't a defect
- 🔒 A security problem goes to [SECURITY.md](SECURITY.md), **not** to a public issue

Please **don't paste your trips into an issue**: screenshots and exports carry real names, dates
and places, and this repository is public. See [CONTRIBUTING.md](CONTRIBUTING.md).

## Is Waypack open source?

Not today. This repository holds the releases, the issue tracker and the docs; the app's code lives
in a private repository. If the code is opened later it will be under a copyleft license (GPL or
AGPL) and it will be announced here.

## Licence

The app is distributed as a compiled binary; all rights reserved. The documents in this repository
may be quoted freely. The privacy policy is in [PRIVACY.md](PRIVACY.md).
