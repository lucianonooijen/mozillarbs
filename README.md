# The Firefox Profile for LARBS

When LARBS installs on a new machine, this Firefox profile is set up.

## Features and settings

- DuckDuckGo is the default search engine for Firefox and VimVixen.
- [AdNauseam](https://adnauseam.io/) installed and enabled for ad-blocking.
- VimVixen installed for vim-like bindings. There are some custom bindings,
  check the add-on preferences for the list.
- A cleanup of the UI.

## Removed anti-features

Here's the junk removed from Firefox:

- Telemetry
- Geolocation
- Push/web notifications
- Websites being able to affect the system cliboard
- Prefetching (Firefox contacting websites you haven't clicked)
- The Pocket

## Installation

This repo should go in `~/.mozilla/firefox/`. If you `cp` or `rsync` it into
that directory, it will overwrite the `profiles.ini` file, which is where you
set your default profile. It won't delete your old profile(s), but if you want
them again, you must modify `profiles.ini` to set them as the `Path` in
`[Profile0]`.
