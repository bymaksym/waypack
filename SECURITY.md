# Security

Waypack's whole argument is that your data cannot leave your phone. A hole in that is the most
serious kind of bug this app can have, and it is worth reporting carefully.

## Reporting a vulnerability

**Do not open a public issue.** Two private channels, either is fine:

- [GitHub private vulnerability reporting](https://github.com/bymaksym/waypack/security/advisories/new)
  — preferred, it keeps the whole thread in one place.
- Email: **bymaksymdev@gmail.com**

Please include what an attacker would need (physical access to an unlocked phone? another app on the
device? a file you open?), the app version from Settings → About, and the Android version.

**What to expect:** this is a one-person project, so no service-level promise — but you will get an
acknowledgement within a few days, and the fix and the release that carries it will be credited to
you unless you'd rather stay anonymous.

## What counts here

Especially interesting:

- Anything that gets data **out of the device** — the app declares no `INTERNET` permission, so a
  path around that is a serious finding.
- **Anything leaving through the system backup that the user did not choose.** The backup rules
  include exactly one folder, `files/cloud/`, and Android excludes everything else on its own. If
  the encrypted database, the settings, the covers or the attachments can be made to travel in a
  system backup or a phone-to-phone transfer, that is a serious finding. So is that folder still
  holding a backup after the user picked "No, thanks".
- Anything readable **at rest**: the database is encrypted with SQLCipher, cover images with the
  Android Keystore, backups with the user's password. Plaintext where there should be none, keys
  recoverable off the device, or leftovers in `-wal`, `-shm`, caches or temporary files.
- The app lock, screenshot blocking or hiding from recents being bypassable.
- Anything that makes an exported backup readable without its password, or the backup written into
  a user-chosen folder readable without the password they set for it.

Known and by design, so not vulnerabilities:

- Opening an attachment in another app writes a temporary decrypted copy through `FileProvider`,
  read-only, and the previous one is deleted on each open. This is stated inside the app.
- Exported backups and `.waypack` files go wherever the user sends them. That is the user's action.
- With **Google backup** chosen, the backup file's password sits beside it in `files/cloud/`, because
  a key that stayed behind would leave the file unreadable on the new phone and the whole option
  pointless. Whoever holds that entire system backup holds both halves; what protects it there is
  Android's own backup encryption, tied to the user's screen lock. This is written on the screen
  before the option is turned on, and the folder option exists for anyone who would rather hold the
  password themselves.
- Someone holding your **unlocked** phone with the app lock turned off can read your trips. So can
  they read your gallery.

## Scope

This repository and the Waypack app published in its releases and on Google Play. The signing
fingerprint of every legitimate build is published in the release notes and shown in the app under
Settings → Privacy → "Verify it yourself"; a build that does not match did not come from here, and
that is worth telling us about too.
