# Userstyles

## ChatGPT

One [Stylus](https://add0n.com/stylus.html) userstyle for ChatGPT with **Catppuccin**, **Rosé Pine**, and **Nord** palettes. Choose a palette and accent in Stylus's style settings; there is only one style to install.

## Install

1. Open [chatgpt.user.less](https://raw.githubusercontent.com/thorgnir/userstyles/main/chatgpt.user.less) with Stylus installed and click **Install style**.
2. Disable older ChatGPT themes to avoid conflicting rules.
3. In Stylus, open this style's settings to choose a palette and accent, then reload `chatgpt.com`.

Available palettes: Catppuccin Latte, Frappé, Macchiato, and Mocha; Rosé Pine Dawn, Main, and Moon; Nord. The accent setting offers the palette default plus red, orange, yellow, green, teal, blue, purple, and pink. Light palettes look best with ChatGPT's light appearance, dark palettes with its dark appearance.

## Why this exists

The earlier [Catppuccin](https://github.com/catppuccin/userstyles/tree/main/styles/chatgpt) and [Rosé Pine](https://github.com/rose-pine/userstyles/tree/main/styles/chatgpt) styles mostly target the old `.light` / `.dark` roots and legacy `--bg-*` colors. The ChatGPT page inspected on 2026-09-28 uses `html.chatgpt-theme[data-theme]` and a newer `--color-*` token set. The Chat/Work switch is now a group labeled `Composer mode` with `aria-pressed` buttons. This style maps the palettes to the new tokens and handles the switch explicitly.

The file is self-contained LESS; no remote CSS or font imports are required. The old token names remain mapped for any dialogs still using them.

## Maintenance

Edit [chatgpt.user.less](chatgpt.user.less) directly. See [AGENTS.md](AGENTS.md) for a checklist when ChatGPT changes its interface again.

## Credits

Palette values come from [Catppuccin](https://github.com/catppuccin/palette), [Rosé Pine](https://rosepinetheme.com/palette/), and [Nord](https://www.nordtheme.com/docs/colors-and-palettes/). This project is available under the [MIT license](LICENSE).
