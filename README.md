# Nothing Light — an Omarchy theme

Bright white theme inspired by Nothing OS: monochrome dot-matrix with a single orange accent (`#e85d04`).

## Install

```
omarchy theme install https://github.com/hell0world69/omarchy-nothing-light-theme
```

## What's inside

- `colors.toml` — the palette; Omarchy generates every app config from it.
- `btop.theme` — hand-patched so btop's network border uses the accent
  instead of red. It does not follow `colors.toml`; update it if you change
  the accent, or delete it to let Omarchy generate one.
- `backgrounds/` — five original dot-matrix wallpapers, a plain white one, and the Omarchy vantablack logo and wordmark with the greys inverted for white (`omarchy theme bg next` to cycle).
- `unlock.png` / `preview-unlock.png` — dot-matrix boot-screen logo
  (`omarchy plymouth set-by-theme nothing-light`).
- `preview.png` — theme picker thumbnail.
- `icons.theme` — grey folder icons (`Tela-circle-grey`). Install them with
  `omarchy pkg add tela-circle-icon-theme-grey`; without the package you
  get the default icons.

## Optional: dot-matrix bar font

The full look uses [Doto](https://fonts.google.com/specimen/Doto) (OFL) in the
bar only. Install the font to `~/.local/share/fonts/`, then add a fontconfig
rule matching `prgname` `quickshell` that replaces `monospace` with `Doto`.
