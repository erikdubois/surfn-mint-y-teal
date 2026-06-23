# Changelog

## 2026.06.23 — split per colour from the LinuxMint upstream

### What Changed

Initial standalone repo. The **Surfn-Mint-Y-Teal** colour variant was generated fresh from
`linuxmint/mint-y-icons` and surfn-ified so it ships as its own package, `surfn-mint-y-teal-icons-git`,
depending on the base `surfn-icons-git`.

### Technical Details

- `usr/share/icons/Mint-Y-Teal/` copied from upstream, dir renamed to `Surfn-Mint-Y-Teal`.
- `index.theme` patched: `Name=Surfn Mint-Y-Teal`, `Inherits=Surfn,Adwaita,gnome,hicolor`.
- `icon-theme.cache` not shipped — the pacman gtk-update-icon-cache hook rebuilds it on install.

### Files Modified

- Initial scaffold + usr/share/icons/Surfn-Mint-Y-Teal/
