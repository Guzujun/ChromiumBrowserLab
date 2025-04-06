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
  <img src="https://private-user-images.githubusercontent.com/126318903/430681436-bac9cd57-7ac7-48bc-8819-ff590412a335.jpg?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NDM5MjAwMDQsIm5iZiI6MTc0MzkxOTcwNCwicGF0aCI6Ii8xMjYzMTg5MDMvNDMwNjgxNDM2LWJhYzljZDU3LTdhYzctNDhiYy04ODE5LWZmNTkwNDEyYTMzNS5qcGc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUwNDA2JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MDQwNlQwNjA4MjRaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1iMWMzMGNlOGZiMWQ0OTgwNzc0OGVjNmY5MmYxNjBkZTRkYmJjODJjYjIzYmQ1MzdhMDM2YWI5NWQyZDRiYzhjJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.TcmTxjJQEkF_Wqz1N7dEq2NjW3tsHrmW1XypsA_5R9Y" width="700"/>

<img src="https://private-user-images.githubusercontent.com/126318903/430681437-0b842421-874e-48d9-94c6-1c73c9edc043.jpg?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NDM5MjAwMDQsIm5iZiI6MTc0MzkxOTcwNCwicGF0aCI6Ii8xMjYzMTg5MDMvNDMwNjgxNDM3LTBiODQyNDIxLTg3NGUtNDhkOS05NGM2LTFjNzNjOWVkYzA0My5qcGc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUwNDA2JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MDQwNlQwNjA4MjRaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT02ZGYzOTA3MDBiZGZlY2YwN2YzZGFlNjFmNzZiZDAyNzg1YTc4NzMxYzg4NDY5ZjEwYmU0MGJjZDVjYTA3Y2FjJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.HPiCugR-UEy81gRs08sf4ioC5y9tBqXoohd8Tiyl6HY" width="700"/>

</p>
My design: By applying a set of self-defined, soft-pink tab group colors that seamlessly blend with the dreamy, pastel-toned background, the theme creates a truly immersive and visually harmonious experience—something not possible with the original set of default tab group colors.

## 🚧 Status

This repository is still under active development for experimentation and proposal purposes. Feel free to explore and leave feedback!

---

## 📄 License

MIT (for demo purposes only)

