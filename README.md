<picture>
  <source media="(prefers-color-scheme: dark)" srcset="docs/plates/hero-dark.png">
  <img alt="Kubet Mono — an original compact monospace for code and terminals" src="docs/plates/hero-light.png" width="1200">
</picture>

# Kubet Mono

An original monospaced typeface for code and terminals, drawn by its own parametric engine. One construction system, one weight, a 600-unit cell that keeps text dense without crowding. Free for personal and commercial use.

**Specimen and type tester:** [dropthetable.com/kubet-mono](https://dropthetable.com/kubet-mono)

## Install

Download the [latest release](https://github.com/kubet/kubet-mono/releases/latest) or take the files from `fonts/`.

```sh
# macOS
curl -LO https://github.com/kubet/kubet-mono/releases/latest/download/KubetMono-Regular.ttf
mv KubetMono-Regular.ttf ~/Library/Fonts/

# Linux
mkdir -p ~/.local/share/fonts
curl -L -o ~/.local/share/fonts/KubetMono-Regular.ttf \
  https://github.com/kubet/kubet-mono/releases/latest/download/KubetMono-Regular.ttf
fc-cache -f
```

Windows: download the TTF, right-click, Install.

```jsonc
// VS Code
"editor.fontFamily": "Kubet Mono",
"editor.fontLigatures": false
```

```ini
# Ghostty
font-family = Kubet Mono
font-feature = ss01   # slashed zero
```

```css
@font-face {
  font-family: "Kubet Mono";
  src: url("KubetMono-Regular.woff2") format("woff2");
  font-weight: 400;
  font-display: swap;
}
```

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="docs/plates/code-dark.png">
  <img alt="TypeScript sample set in Kubet Mono" src="docs/plates/code-light.png" width="1200">
</picture>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="docs/plates/term-dark.png">
  <img alt="Terminal sample: box drawing table, block progress bars, braille spinner, Powerline prompt" src="docs/plates/term-light.png" width="1200">
</picture>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="docs/plates/pairs-dark.png">
  <img alt="Identity pairs: 0O, 1lI|, rn m, cl d, vv w, 5S 2Z, 8B 6b, 9g q, brackets, points, quotes, dashes" src="docs/plates/pairs-light.png" width="1200">
</picture>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="docs/plates/water-dark.png">
  <img alt="Waterfall from 9 to 24 px" src="docs/plates/water-light.png" width="1200">
</picture>

## Datasheet

| | |
| --- | --- |
| Family · style | Kubet Mono · Regular (400), upright |
| Version | 0.001 · source build `af6f2d0` · 2026-10-26 |
| Units per em | 1000 |
| Advance width | 600, fixed; no kerning |
| Cap height · x-height | 700 · 524 |
| Ascender (l) · descender | 815 · −230 |
| Line height | 1.332 em (1102 / −230) |
| Stem | 92 units |
| Glyphs · codepoints | 828 · 783 |
| OpenType | `ccmp`, `ss01` slashed zero, `mark`, `mkmk` |
| Hinting | `prep` + `gasp`: grayscale antialiasing at every size |
| Embedding | `fsType` 0, installable |

### Coverage

| Block | Cells |
| --- | --- |
| Basic Latin | 95 / 95 |
| Latin-1 Supplement | 96 / 96 |
| Latin Extended-A | 128 / 128 |
| Latin Extended-B digraphs Ǆ–ǌ | 9 / 9 |
| Combining marks | 13 |
| Arrows, math, bullet, ellipsis | 16 |
| Box Drawing | 128 / 128 |
| Block Elements | 32 / 32 |
| Braille Patterns | 256 / 256 |
| Powerline (private use) | 8 |

Languages: English, German, French, Spanish, Portuguese, Italian, Dutch, Serbian, Croatian, Slovene, Polish, Czech, Slovak, Hungarian, Romanian, Turkish and the rest of Latin-1 plus Extended-A.

### Files

| File | Size | SHA-256 |
| --- | --- | --- |
| `fonts/ttf/KubetMono-Regular.ttf` | 121,656 B | `7b9720b1adefa501c7b2f7875834b814a309ede8be82b79118d3d85f50e1cf12` |
| `fonts/otf/KubetMono-Regular.otf` | 76,024 B | `efed7dda6baf1c131976df397b1093161e42f428b67236d05250347a781780d2` |
| `fonts/web/KubetMono-Regular.woff2` | 26,900 B | `2fc7f1f726fe0d8e280e00269233d944e5d37a81c28cde9d15e9ef4e85c1b35f` |

## Design notes

- **Fixed cells.** Every spacing glyph has one advance; marks have zero. No kerning or contextual alternates rescue a bad default. The grid is the contract.
- **Round but serious.** Gently squared superelliptic rounds, flat precise terminals, nothing bubbly. The capital O and lowercase o are the master rounds; every curve derives from them.
- **Letter fit.** The gap between two `n` is about 0.70 of the counter width, inside the 0.65–0.80 band that compact monospaces share, so text is dense without crowding.
- **Identity by shape, not width.** Zero carries an oblong centre mark (slash via `ss01`), the lowercase l hooks, the capital I has slabs, the one has a flag and a foot.
- **Original construction.** Only Kubet's programs and parameters produce ink. Other monospaces were measured as peers, never traced.

## License

[Kubet Mono License 1.0](LICENSE.md). In short: use it anywhere, embed it, share it unmodified, modify it for yourself. Don't sell it, don't publish derivatives under the Kubet name, don't train type-generating models on it. No warranty.

Kubet Mono © 2026 Vukašin Kubet · [drop.table](https://dropthetable.com)
