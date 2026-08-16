# moon-flavor

*a moonlight-flavored Pi-style theme for DeepSeek Harness.*

A theme plugin for the [DeepSeek Harness](https://github.com/deepseek-ai/dsh) web UI,
recreating the [pi.dev](https://pi.dev) design language — moonstone-cream surfaces,
serif italics, hazy-blue accents, sharp corners, and terminal-flavored motion.

## Palette

| Role | Light | Dark |
|---|---|---|
| Base | `#EBE7E4` moonstone cream | `#1B1A18` warm charcoal |
| Accent | `#6A9FCC` hazy blue | `#7FB0D8` |
| Ink | `#384251` blue-grey | `#E8E4DE` |

## Install

```bash
npm install moon-flavor
```

Then register it in your profile's `cordis.patch.yml`:

```yaml
- insert:
    - id: moon-flavor
      name: 'moon-flavor'
```

Restart `dsh web` and hard-refresh (Cmd+Shift+R).

## Typefaces

The theme leans on **Plantin** (a serif with old-style character) for latin text,
falling back through Georgia / Times New Roman, with **Songti SC / SimSun** for CJK
so Chinese surfaces keep the same serif flavor.

> Plantin is a commercial face and is **not bundled**. macOS ships it;
> other platforms fall back to Georgia (latin) and Songti/SimSun (CJK).

## Compatibility

- Built against `@deepseek-ai/dsh@0.1.0-rc.6`
- Stable across versions: the `--dsw-alias-*` / `--dsw-static-*` design tokens
- Version-sensitive: hashed css-modules class names (`.hHd-Xa_brand`, `.wSkVaW_root`, …) may drift on dsh upgrades

## License

MIT
