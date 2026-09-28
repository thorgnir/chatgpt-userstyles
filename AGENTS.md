# Agent guidance

This repository currently contains one self-contained Stylus LESS userstyle: `chatgpt.user.less`. It supports Catppuccin, Rosé Pine, and Nord through Stylus `@var select` settings. Keep the ChatGPT theme as one installable file; add future palettes to its palette map and reuse the shared UI rules. Other sites may have separate userstyle files.

## When ChatGPT changes its UI

1. Reproduce the problem in a browser with Stylus. Disable other ChatGPT styles first.
2. Inspect the live DOM and computed CSS. Record the current theme marker, accessible attributes, and relevant CSS custom properties. Prefer stable attributes and design tokens over hashed classes and Tailwind utility names.
3. Update the palette-to-token mapping and targeted selectors in `chatgpt.user.less`. Keep the file self-contained, without remote imports, fonts, scripts, or extension APIs.
4. Compile the LESS for a light palette, a dark palette, and Nord with a non-default accent. Confirm there are no unresolved variables or syntax errors.
5. Verify the home page, an existing conversation, composer, sidebar, Chat/Work switch, a menu or dialog, and a code block when available. Check Firefox and Chromium if accessible.
6. Confirm the UserCSS metadata still has a working raw-file update URL. Explain any view or browser that could not be checked.

Preserve ChatGPT's layout, keyboard focus indicators, state transitions, and accessibility attributes. Avoid broad `!important` rules and selectors based solely on generated class names. Palette values are upstream colors; keep attribution in README.
