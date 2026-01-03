# Catppuccin Wallpapers

Minimal wallpapers featuring the [Catppuccin](https://catppuccin.com/) color palette.

## Desktop (2560x1600)

<table>
  <tr>
    <td align="center">
      <img src="./desktop/catppuccin-latte.png" width="100%" />
      <br />
      <b>Latte</b> <code>#eff1f5</code>
    </td>
    <td align="center">
      <img src="./desktop/catppuccin-frappe.png" width="100%" />
      <br />
      <b>Frappe</b> <code>#303446</code>
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="./desktop/catppuccin-macchiato.png" width="100%" />
      <br />
      <b>Macchiato</b> <code>#24273a</code>
    </td>
    <td align="center">
      <img src="./desktop/catppuccin-mocha.png" width="100%" />
      <br />
      <b>Mocha</b> <code>#1e1e2e</code>
    </td>
  </tr>
</table>

## Phone (1170x2532)

### Plain (No Logo)

| Latte | Frappe | Macchiato | Mocha |
|:-----:|:------:|:---------:|:-----:|
| <img src="./phone/plain/catppuccin-latte.png" width="150" /> | <img src="./phone/plain/catppuccin-frappe.png" width="150" /> | <img src="./phone/plain/catppuccin-macchiato.png" width="150" /> | <img src="./phone/plain/catppuccin-mocha.png" width="150" /> |
| `#eff1f5` | `#303446` | `#24273a` | `#1e1e2e` |

## How to Generate

These wallpapers were generated using **ImageMagick**.

### Prerequisites

```bash
# macOS (Homebrew)
brew install imagemagick
```

### Desktop Wallpapers

```bash
# Latte (Light)
magick -size 2560x1600 xc:"#eff1f5" \
  \( assets/catppuccin-logo.png -resize 400x400 \) \
  -gravity center -composite \
  desktop/catppuccin-latte.png

# Frappe
magick -size 2560x1600 xc:"#303446" \
  \( assets/catppuccin-logo.png -resize 400x400 \) \
  -gravity center -composite \
  desktop/catppuccin-frappe.png

# Macchiato
magick -size 2560x1600 xc:"#24273a" \
  \( assets/catppuccin-logo.png -resize 400x400 \) \
  -gravity center -composite \
  desktop/catppuccin-macchiato.png

# Mocha (Darkest)
magick -size 2560x1600 xc:"#1e1e2e" \
  \( assets/catppuccin-logo.png -resize 400x400 \) \
  -gravity center -composite \
  desktop/catppuccin-mocha.png
```

### Phone Wallpapers (Plain)

```bash
# Latte (Light)
magick -size 1170x2532 xc:"#eff1f5" phone/plain/catppuccin-latte.png

# Frappe
magick -size 1170x2532 xc:"#303446" phone/plain/catppuccin-frappe.png

# Macchiato
magick -size 1170x2532 xc:"#24273a" phone/plain/catppuccin-macchiato.png

# Mocha (Darkest)
magick -size 1170x2532 xc:"#1e1e2e" phone/plain/catppuccin-mocha.png
```

## Credits

- Logo from [Catppuccin](https://github.com/catppuccin/catppuccin)
- Colors from [Catppuccin Palette](https://catppuccin.com/palette)
