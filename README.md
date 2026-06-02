# KW Icon

KW Icon is a tiny macOS menu bar app that shows the current ISO calendar week as
`KW 23` in the menu bar.

macOS does not let third-party apps force an exact menu bar position beside
Apple's battery, Wi-Fi, and clock items. After launching the app, hold Command
and drag `KW 23` to the position you prefer.

## Existing App Option

If you just want a finished app, install
[Week Number by Sindre Sorhus](https://sindresorhus.com/week-number). It is free
and shows the current week number in the menu bar. The current App Store version
requires macOS 26 or later; older versions for macOS 15 and macOS 14 are linked
from the app's website.

## Build

```sh
./scripts/build.sh
```

The app bundle is created at:

```text
dist/KW Icon.app
```

Run it without installing:

```sh
open "dist/KW Icon.app"
```

## Install

Install to `~/Applications` and launch:

```sh
./scripts/install.sh
```

Install and start automatically at login:

```sh
./scripts/install.sh --login
```

Uninstall the login item:

```sh
./scripts/install.sh --uninstall-login
```

Then delete `~/Applications/KW Icon.app` if you no longer want the app.
