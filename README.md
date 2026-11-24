# Mirrored Pages

![Mirrored Pages in dark mode](screenshot.png)

A silver-mirror theme for [Obsidian](https://obsidian.md): deep, dark slate glass in dark mode, brushed silver in light mode, and serif headings with a reflected rule beneath them.

Made for [The Mirrored Realms](https://github.com/ShadowOkami4/Mirrorgate), a tabletop RPG setting written as an Obsidian vault, but it works in any vault.

## Features

- **Dark and light modes.** Slate, obsidian or pewter surfaces in the dark; brushed silver in the light.
- **Silver headings.** A soft sheen on titles and a mirrored double rule under the first two heading levels.
- **Callouts framed like small mirrors:** a tinted title band, a round icon badge, silver corner brackets and a diagonal glint. Every callout type has its own colour.
- **Mirror-pane blockquotes** with a large quotation mark and a double accent bar.
- **Mirror-shard separators:** `---` becomes a silver line with a glowing diamond.
- **Frosted-glass menus and pop-ups**, with framed hover previews.
- **A livelier workspace:** glowing active file and accent-lined active tab, tinted folder icons, ribbon icons that glow on hover, a glass status bar.
- **Text details:** links that glow on hover, diamond list bullets, glowing checkboxes, tag pills, soft highlight glow, code chips and accent footnote numbers.
- **Tables and Bases:** small-caps headers with an accent rule, striped rows, hover highlight, a tinted Bases toolbar.
- **Frames for properties, embedded notes, images and code blocks.**
- **A `[!gm]` callout** for Game Master notes, with a *GM only* corner ribbon.
- **A `[!player]` callout** for text players may read, drawn as a card with a *Player info* corner ribbon.
- **Section cards.** Add `cssclasses: hub` to a note, and each list under a heading becomes a grid of cards in reading view: icon badge, coloured top edge, subtitle and a large faded icon. Text after the link, such as `<small>Places and maps</small>`, becomes the subtitle.
- **A small cracked mirror-shard emblem** in the bottom-right corner of every note.
- **Night-sky graph view behind cracked mirror glass** in dark mode, and a pale dawn sky in light mode.
- **Atlas VTT support.** The [Atlas VTT](https://github.com/ByteMirror/atlas-vtt) plugin picks up the theme's colours, accents and dice font.
- **No external requests.** No web fonts or images are loaded; headings use serif fonts already on your system.

## Settings

Install [Style Settings](https://github.com/mgmeyers/obsidian-style-settings) to change:

| Setting | Options |
| --- | --- |
| Mirror accent | any colour, separately for dark and light |
| GM callout colour | any colour, separately for dark and light |
| Player info colour | any colour, separately for dark and light |
| Surface | slate, obsidian, pewter |
| Heading style | serif or sans-serif |
| Serif body text | on / off |
| Page width | 560–1100 px |
| Heading sheen, reflected rule, page emblem, night sky, mirror cracks | on / off |
| Glass blur | 0–24 px |

## Requirements

Obsidian 1.15 or newer.

## Installing

**From Obsidian:** Settings → Appearance → Themes → Manage → search for *Mirrored Pages*. *(Pending review for the community theme list.)*

**By hand:** copy `theme.css` and `manifest.json` into `<your vault>/.obsidian/themes/Mirrored Pages/`, then choose *Mirrored Pages* under Settings → Appearance → Themes.

## GM and player callouts

```markdown
> [!gm]- GM only
> The innkeeper is the thief.

> [!player] What players know
> The inn is warm, cheap and never empty.
```

## Custom card colours and icons

Each card reads two variables, so a CSS snippet in your vault can give a card its own look by matching the link name:

```css
body .hub .el-ul > ul > li:has(> a.internal-link[data-href="Atlas"]) {
  --mp-card-color: #4a90e2;
  --mp-card-icon: url("data:image/svg+xml;utf8,…");  /* any SVG; used as a mask */
}
```

## License

[MIT](LICENSE) © Okami. The default card icon is from [Lucide](https://lucide.dev) (ISC License).
