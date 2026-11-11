<p align="center">
  <img src="https://img.shields.io/badge/Millennium-141218?style=for-the-badge&logo=steam&logoColor=C4A8E2"/>
  <img src="https://img.shields.io/badge/Lotus_Purple-141218?style=for-the-badge&logo=codeforces&logoColor=C4A8E2"/>
</p>

<h1 align="center">Lotus Steam</h1>

A purple glass theme for the Steam client, loaded with
[Millennium](https://github.com/SteamClientHomebrew/Millennium). It covers the
library, the store, the friends list, the chat and Big Picture Mode.

## Install

Millennium must be installed and working first.

From Millennium's theme browser, add the repository
`https://github.com/LotsV8pro/lotus-steam` and install `Lotus Purple`. The
`skin.json` in the root tells Millennium which files to inject.

By hand:

```bash
git clone https://github.com/LotsV8pro/lotus-steam.git "$HOME/.steam/steam/steamui/skins/Lotus"
```

Then open Steam, go to Millennium, Themes, select `Lotus Purple` and refresh.
`~/.steam/steam` is a symlink to `~/.local/share/Steam` on most installs, so
either path works.

## Files

| File | What it styles |
|---|---|
| `skin.json` | Millennium metadata: name, author, colours, conditions |
| `colors.css` | Colour variables for the rest of the files |
| `libraryroot.custom.css` | Library, shelves, game pages |
| `friends.custom.css` | Friends list and chat |
| `bigpicture.custom.css` | Big Picture Mode |
| `webkit.css` | Store and other embedded web views |

The colours are declared once in `colors.css`. Change them there rather than in
the other files.

## Palette

| Token | Hex |
|---|---|
| Accent | `#C4A8E2` |
| Accent dim | `#8C7AA6` |
| Accent dark | `#383048` |
| Text | `#D8D0E8` |
| Text dim | `#887898` |
| Background | `#141218` |
| Background alt | `#1C1A22` |
| Background light | `#282430` |

## Compatibility

- Steam desktop client on Linux, with Millennium
- Big Picture Mode, with some elements left at their default shape

Valve changes the client markup often. When a section stops following the
theme, the selector that matched it has probably been renamed; the fix belongs
in the file that styles that section, not in `colors.css`.

## Related repos

- [lotus-discord](https://github.com/LotsV8pro/lotus-discord): the same palette for Discord
- [lotus-spotify](https://github.com/LotsV8pro/lotus-spotify): the same palette for Spotify
- [Lotus-Arch](https://github.com/LotsV8pro/Lotus-Arch): the desktop it matches

## License

MIT.
