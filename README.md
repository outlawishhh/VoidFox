# VoidFox

A dark-themed custom Firefox new tab page with structured quick-launch shortcuts and a minimal aesthetic.

## Overview

VoidFox replaces the default Firefox startpage with a lightweight, high-contrast dashboard. Built around a dark obsidian palette and subtle neon accent highlights, it features an integrated search bar, an embedded clock widget, image preview framing, and categorized quick-launch navigation columns.

## Preview

https://github.com/user-attachments/assets/46c9f9d4-d269-4ad6-a6d3-a222719636cf

## Features

* **High-Contrast Dark Aesthetic:** Built on a dark visual palette with dynamic CSS hover states and custom glow effects.
* **Integrated Search:** Embedded web search form supporting instant queries via Google.
* **Categorized Quick Launch:** Organized column structures for quick access to frequent links across distinct categories.
* **Embedded Widgets:** Clean, centered clock interface powered by standard web embeds.
* **Customizable Assets:** Configurable background media slot and easily swappable local image presets.

## Installation

### Requirements

* [Firefox Browser](https://www.mozilla.org/en-US/firefox/new/)
* [New Tab Override Add-on](https://addons.mozilla.org/en-US/firefox/addon/new-tab-override/)

### Setup Instructions

1. Install the **[New Tab Override](https://addons.mozilla.org/en-US/firefox/addon/new-tab-override/)** extension from the Mozilla Add-ons store.
2. Open the extension settings by clicking the **New Tab Override** icon in your browser toolbar (or via `about:addons`).
3. Under the **Option** menu, set the redirect type to **Custom URL**.
4. In the URL field, paste your GitHub Pages deployment link:
```text
https://outlawishhh.github.io/VoidFox/

```


5. Open a new tab to verify the page loads automatically.

## Customization

### Links & Collections

Open `index.html` in any text editor to modify the links, titles, and target URLs inside the `.collection-links-wrapper` blocks:

```html
<li class="collection-links-wrapper">
  <h3 class="collection-title">Category Title</h3>
  <ul class="links-container">
    <li class="link-wrapper" tabindex="0">
      <a href="https://example.com" class="link" tabindex="-1">Link Name</a>
    </li>
  </ul>
</li>

```

### Color Palette & Accents

Adjust the root CSS variables at the top of the stylesheet to customize background tones and hover highlights:

```css
:root {
  --main-bg-color: 0, 0, 0 !important;
  --main-fg-color: 255, 255, 255 !important;
  --main-accent: 140, 0, 26 !important;
  --accent-1: 167, 192, 128 !important;
  --accent-2: 230, 126, 128 !important;
}

```

## How It Works

* **Pure Web Standards:** Operates purely on native HTML5 and CSS3 with zero heavy JavaScript dependencies required for layout rendering.
* **Responsive Styling:** Flexible CSS Flexbox and Grid containers scale cleanly across different screen resolutions.

## Credits

* **Created by:** Outlawishhh
* Designed and implemented from scratch.

## License

Copyright (C) 2026 Outlawishhh

Licensed under the GNU General Public License v3.0 (GPL-3.0).

You are free to use, modify, and redistribute this project under the terms of the GPL-3.0 license. Any distributed modifications must also remain open source and retain attribution to the original author.

See the LICENSE file for details.
