# VoidFox

A dark-themed custom Firefox new tab page with structured quick-launch shortcuts and a minimal aesthetic.

## Overview

VoidFox replaces the default Firefox startpage with a lightweight, high-contrast dashboard. Built around a dark obsidian palette and subtle neon accent highlights, it features an integrated search bar, an embedded clock widget, image preview framing, and organized quick-launch navigation columns. Out of the box, it comes pre-configured with essential web shortcuts for social media, development tools, streaming services, and utility platforms.

## Preview

https://github.com/user-attachments/assets/6ce433b3-cb75-4cab-ab43-c406b9f3ac24

## Features

* **High-Contrast Dark Aesthetic:** Built on a dark visual palette with dynamic CSS hover states and custom glow effects.
* **Integrated Search:** Embedded web search form supporting instant queries via Google.
* **Categorized Quick Launch:** Pre-configured shortcuts across five structured categories (*Socials*, *Dev*, *Media*, *Tools*, and *Misc*).
* **Embedded Widgets:** Clean, centered clock interface powered by standard web embeds.
* **Customizable Assets:** Configurable background media slot and easily swappable local image presets.

## Installation & Setup

Choose one of the methods below depending on whether you want to use the default setup, host your own customized version online, or run a local file.

### Prerequisites

* [Firefox Browser](https://www.mozilla.org/en-US/firefox/new/)
* [New Tab Override Add-on](https://addons.mozilla.org/en-US/firefox/addon/new-tab-override/)

---

### Option 1: Quick Setup 

If you want to use VoidFox immediately with the clean default bookmarks:

1. Install the **[New Tab Override](https://addons.mozilla.org/en-US/firefox/addon/new-tab-override/)** extension in Firefox.
2. Open extension settings by clicking the **New Tab Override** icon in your toolbar.
3. Under the **Option** dropdown, select **Custom URL**.
4. In the **URL** field, paste the direct hosted deployment link:
```text
https://outlawishhh.github.io/VoidFox/
```


5. Click the blue **Save rule** button.
6. Open a new tab to verify.

---

### Option 2: Custom Setup

If you want to customize your own bookmarks and host your personalized dashboard:

1. **Fork** this repository to your personal GitHub account.
2. Edit `index.html` inside your fork to replace or add your personal links and categories.
3. In your forked repository, navigate to **Settings** $\rightarrow$ **Pages**.
4. Under **Source**, select **Deploy from a branch** $\rightarrow$ `main` branch $\rightarrow$ `/(root)` folder, then click **Save**.
5. Copy your generated GitHub Pages link:
```text
https://<your-username>.github.io/VoidFox/
```


6. Open **New Tab Override** settings in Firefox, set the **Option** dropdown to **Custom URL**.
7. Paste your personalized URL in the **URL** field, then click the blue **Save rule** button.

---

### Option 3: Local Setup

If you prefer running your startpage locally without hosting it online:

1. Clone or download this repository to your local machine:
```bash
git clone https://github.com/outlawishhh/VoidFox.git
```


2. Edit `index.html` in your text editor to customize your links.
3. Open **New Tab Override** settings in Firefox.
4. Under the **Option** dropdown, select **Local file**.
5. Click to choose the local `index.html` file on your computer.
6. Click the blue **Save rule** button to apply your changes.

---

## Customization

### Editing Links & Categories

Open `index.html` in any editor to modify titles, links, or URLs inside the `.collection-links-wrapper` blocks:

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

Adjust the root CSS variables at the top of the stylesheet to modify background tones and hover accents:

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
