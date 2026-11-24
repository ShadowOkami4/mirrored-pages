# Mirrored Pages

![Mirrored Pages in dark mode](screenshot.png)

A silver-mirror theme for [Obsidian](https://obsidian.md): deep slate glass in dark mode, brushed silver in light mode, and serif headings with a reflected rule beneath them.

Made for [The Mirrored Realms](https://github.com/ShadowOkami4/Mirrorgate), a tabletop RPG setting written as an Obsidian vault, but it works in any vault.

## Features

- **Dark and light modes.** Slate, obsidian or pewter surfaces in the dark; brushed silver in the light.
- **Silver headings.** A soft sheen on titles and a mirrored double rule under the first two heading levels.
- **Frosted-glass callouts, menus and pop-ups.**
- **A `[!gm]` callout** for Game Master notes, coloured separately from other callouts.
- **Hub notes as cards.** Add `cssclasses: hub` to a note, and the list under each heading is shown as a grid of glass cards in reading view.
- **Starfield graph view** in dark mode.
- **Atlas VTT support.** The [Atlas VTT](https://github.com/ByteMirror/atlas-vtt) plugin picks up the theme's colours, accents and dice font.
- **No external requests.** No web fonts or images are loaded; headings use serif fonts already on your system.

## Settings

Install [Style Settings](https://github.com/mgmeyers/obsidian-style-settings) to change:

| Setting | Options |
| --- | --- |
| Mirror accent | any colour, separately for dark and light |
| GM callout colour | any colour, separately for dark and light |
| Surface | slate, obsidian, pewter |
| Heading style | serif or sans-serif |
| Serif body text | on / off |
| Page width | 560–1100 px |
| Heading sheen, reflected rule, starfield | on / off |
| Glass blur | 0–24 px |

## Installing

**From Obsidian:** Settings → Appearance → Themes → Manage → search for *Mirrored Pages*. *(Pending review for the community theme list.)*

**By hand:** copy `theme.css` and `manifest.json` into `<your vault>/.obsidian/themes/Mirrored Pages/`, then choose *Mirrored Pages* under Settings → Appearance → Themes.

## GM callout

```markdown
> [!gm]- GM only
> The innkeeper is the thief.
```

## License

[MIT](LICENSE) © Okami
