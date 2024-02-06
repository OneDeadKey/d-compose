# D‑Compose
A cross-platform [Compose key](https://en.wikipedia.org/wiki/Compose_key) for any keyboard layout.

There’s nothing to see yet.

## Idea

- grab Compose key sequences from XOrg
- extend them with *ASCII-only* sequences
- (maybe?) make a quick Rust/Tauri UI to browse, filter, and customize these sequences.

The implementation could rely on:

- AHK on Windows (deadkey-chaining is hacky *at best* on this platform)
- `~/Library/KeyBindings/DefaultKeyBinding.dict` on macOS
- XCompose on Linux (no shit, Sherlock?)

… unless we hit the [rusty road](https://github.com/espanso/espanso) and come up
with our own implementation.

## Links

- https://www.x.org/releases/current/doc/libX11/i18n/compose/en_US.UTF-8.html
- https://cgit.freedesktop.org/xorg/lib/libX11/plain/nls/en_US.UTF-8/Compose.pre

Windows

- https://github.com/samhocevar/wincompose
- https://www.autohotkey.com/board/topic/92511-wincompose-a-robust-compose-key-for-windows/
- https://github.com/jmcwilliams403/XComposeAHKv2
- https://github.com/DreymaR/BigBagKbdTrixPKL/blob/master/Files/_eD_Compose.ini

macOS

- https://pypi.org/project/gen-compose/
- https://github.com/Granitosaurus/macos-compose
- https://github.com/rastislavcore/osx-compose-key

Linux

- https://wiki.debian.org/XCompose
- https://help.ubuntu.com/community/ComposeKey
- https://help.ubuntu.com/community/GtkComposeTable
