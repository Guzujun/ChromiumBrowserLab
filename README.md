# ChromiumBrowserLab

This repository contains experimental modifications to the Chromium browser UI, focusing on two key features:

- 🖱️ Middle-click to close a **tab group**
- 🎨 API support for **custom tab group colors** in themes

These changes are intended as part of a Google Summer of Code (GSoC) proposal for improving the Chromium theming system.

---

## 🔧 Features

### 1. Middle-click to Close Tab Group
Implemented in `group_header.cc`, this feature allows users to middle-click on a tab group header to close all tabs within that group instantly.

### 2. Custom Tab Group Colors (Theme API)
Added support for new manifest keys (`"tab_group_custom0"` to `"tab_group_custom8"`) that allow theme developers to define their own tab group color palette, overriding the default 9-color system.

---

## 📁 Project Structure

```
chromium/
└── src/
    └── chrome/
        └── *browser(current)/
            └── themes/
                ├── browser_theme_pack.cc
                └── theme_properties.h
            └── ui/
                ├── color/
                │   └── chrome_color_id.h
                └── views/
                    └── tabs/
                        └── tab_group_header.cc

```


---

## ✨ Demo

Here’s a comparison showing the default 9-color tab group palette and the newly applied soft-pink custom color from a user-defined theme:

<p align="center">
  <img src="https://your.image.hosting/link/to/image.png" width="700"/>
</p>

---

## 🚧 Status

This repository is still under active development for experimentation and proposal purposes. Feel free to explore and leave feedback!

---

## 📄 License

MIT (for demo purposes only)

