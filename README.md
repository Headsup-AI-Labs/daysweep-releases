# Daysweep releases

The update feed for [Daysweep](https://daysweep.ai), a Mac app that reads WhatsApp,
Gmail and Slack on the machine you already use and keeps what you owe people in one
list.

This repository is public so the app can reach `appcast.xml` without credentials.
The source lives elsewhere and is private. Nothing here is secret.

- **`appcast.xml`** — the feed Sparkle reads. Each entry names a version and the DMG
  that carries it.
- **Releases** — the signed, notarized DMGs themselves.

Every entry carries an EdDSA signature. The app refuses any download whose signature
does not match the public key inside the installed copy, so a compromise of this
repository cannot cause an update to be installed.

To install Daysweep for the first time, download the newest DMG from Releases. After
that the app updates itself.
