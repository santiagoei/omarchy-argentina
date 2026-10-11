# Argentina — Omarchy theme

A dark Omarchy theme inspired by the alternate kit of the Asociación del Fútbol Argentino: deep navy surfaces, celeste accents, and the gold of the Sol de Mayo.

![preview](preview.png)

## Install

```bash
omarchy theme install https://github.com/santiagoei/omarchy-argentina.git
omarchy theme set argentina
```

## Palette

| Token | Color | Inspiration |
|---|---|---|
| accent | `#75aadb` | Celeste |
| background | `#0c1c30` | Tercera camiseta (navy) |
| foreground | `#eaf1f8` | Blanco |
| yellow | `#f6b40e` | Sol de Mayo |
| green | `#63c7a3` | Campo de juego |
| red | `#e57382` | Papel picado |
| brown | `#8a6a48` | Pelota de cuero |

Window borders use a celeste→white gradient, like the stripes of the home kit.

## Backgrounds

20 photos of Argentina — Buenos Aires (the Obeliscos, Congreso, Caminito,
the neighborhoods, Mar del Plata), Iguazú, El Calafate, Aconcagua, Los
Alerces, Jujuy's Siete Colores and estadio, the seven lakes of Neuquén,
Córdoba, a map, and one for Diego. Filenames carry their priority tier,
so the alphabetical cycle runs first-pick first: `01_arg_bsas_obelisco.jpg`
opens the theme. The light sister shares this exact pool, renumbered
around its own opener.

## Sister theme

[omarchy-argentina-light](https://github.com/santiagoei/omarchy-argentina-light.git) — the home kit version: celeste and white.

## Development

This repo root is the theme directory itself; `omarchy theme install` clones it to `~/.config/omarchy/themes/<name>`. Everything here is color data: no `*.lua`, terminal configs, or `vscode.json` are shipped (those are dropped by the installer and regenerated from `colors.toml`).

To hack on it locally:

```bash
git clone <this-repo> ~/code/omarchy-argentina
ln -s ~/code/omarchy-argentina ~/.config/omarchy/themes/argentina
omarchy theme set argentina
```

Remove the symlink before testing `omarchy theme install` — the installer deletes the destination directory.

## License

MIT
