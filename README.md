<div align="center">

# Waypack

**A packing and trip organizer that cannot go online.**

[Download the latest APK](https://github.com/bymaksym/waypack/releases/latest) ·
[Report a bug](https://github.com/bymaksym/waypack/issues/new?template=bug_report.yml) ·
[Privacy policy](PRIVACY.md) ·
[Leer en español](README.es.md)

</div>

---

Waypack organizes your trips and what you pack for them — by day, by bag, by person — and every
byte of it stays on your phone. There is no account, no sync, no server, no ads and no analytics.

Not "we promise we don't send your data". **The app has no way to send it**: it ships with the
`INTERNET` permission explicitly removed, so even if it tried, Android would refuse.

> This repository is the home of Waypack's **releases, bug reports and discussions**. The app's
> source code is not public (yet). See [Is Waypack open source?](#is-waypack-open-source) below.

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
- Legs, places by day, documents and attachments — your passport and your track live with the trip,
  not in a Downloads folder with forty other files.
- Encrypted backup with your own password, and a file you can hand to whoever travels with you.
- English, Spanish, Russian and Ukrainian, with an in-app language switch.
- Screenshot blocking, hiding from recents, and an app lock behind your phone's own credential.

## Privacy, in checkable form

| | |
| --- | --- |
| Permissions | **None.** `INTERNET` is explicitly removed from the manifest |
| Database | Encrypted with SQLCipher |
| Cover photos | Encrypted with the Android Keystore |
| Backups | Encrypted with a password you choose |
| Android auto-backup | Off (`allowBackup=false`) — nothing leaves in a system cloud copy |
| Google Play Services | Not used, not needed. Runs on GrapheneOS and de-Googled phones |
| Analytics, crash reporting, ads | None |

Inside the app, **Settings → Privacy → "Verify it yourself"** shows the permissions the running app
declares and its signing fingerprint, so you can check all of the above without trusting this page.

## Install

**Requires Android 8.0 (API 26) or newer.**

- **Direct download** — grab `app-release.apk` from the
  [latest release](https://github.com/bymaksym/waypack/releases/latest) and open it.
- **[Obtainium](https://github.com/ImranR98/Obtainium)** — point it at this repository and it will
  track new versions for you. The APK's filename stays the same on purpose so that this keeps
  working.

### Verify what you downloaded

Every release lists two fingerprints. Both are worth thirty seconds:

```
# 1. The file is the one that was published
sha256sum app-release.apk        # must match the .sha256 in the release

# 2. It was signed with Waypack's key and not repackaged by someone else
apksigner verify --print-certs app-release.apk
```

That second fingerprint is the one the app shows you under **Verify it yourself**. If the three
values — the release notes, your download, and the running app — don't all agree, whatever you
installed did not come from here.

## Report a bug or ask for something

- 🐞 [Bug report](https://github.com/bymaksym/waypack/issues/new?template=bug_report.yml)
- 💡 [Feature request](https://github.com/bymaksym/waypack/issues/new?template=feature_request.yml)
- 💬 [Discussions](https://github.com/bymaksym/waypack/discussions) — questions, packing setups,
  anything that isn't a defect
- 🔒 A security problem goes to [SECURITY.md](SECURITY.md), **not** to a public issue

One request that matters here more than in most apps: **don't paste your trips into an issue**.
Screenshots and exports carry real names, dates and places. Nothing of that helps a bug report, and
this repository is public. See [CONTRIBUTING.md](CONTRIBUTING.md).

## Is Waypack open source?

Not today. This repository holds the releases, the issue tracker and the docs; the app's code lives
in a private repository.

That is a decision about the code, not about the promise: nothing here depends on trusting the
author's word. The permission list is enforced by Android, the Data safety card on Google Play is
filled in by Google, and the signing fingerprint is checkable from the app itself. If the code is
opened later it will be under a copyleft license (GPL or AGPL) and it will be announced here.

## Licence

The app is distributed as a compiled binary; all rights reserved. The documents in this repository
(this README, the privacy policy) may be quoted freely.
