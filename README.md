# Catppuccin Wallpapers

Minimal wallpapers featuring the [Catppuccin](https://catppuccin.com/) color palette for MacBook (2560x1600).

## Previews

<table>
  <tr>
    <td align="center">
      <img src="./catppuccin-latte-wallpaper.png" width="100%" />
      <br />
      <b>Latte</b> <code>#eff1f5</code>
    </td>
    <td align="center">
      <img src="./catppuccin-frappe-wallpaper.png" width="100%" />
      <br />
      <b>Frappé</b> <code>#303446</code>
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="./catppuccin-macchiato-wallpaper.png" width="100%" />
      <br />
      <b>Macchiato</b> <code>#24273a</code>
    </td>
    <td align="center">
      <img src="./catppuccin-mocha-wallpaper.png" width="100%" />
      <br />
      <b>Mocha</b> <code>#1e1e2e</code>
    </td>
  </tr>
</table>

## How to Generate

These wallpapers were generated using **ImageMagick**. You can recreate them or customize the size/colors using the following commands:

### 1. Prerequisites
Install ImageMagick:
```bash
# macOS (Homebrew)
brew install imagemagick
```

### 2. Download Logo
```bash
curl -o catppuccin-logo.png "https://upload.wikimedia.org/wikipedia/commons/7/7b/Catppuccin_Logo.png"
```

### 3. Generate Wallpapers
Run the following commands to generate the wallpapers (2560x1600):

```bash
# Latte (Light)
magick -size 2560x1600 xc:"#eff1f5" \
  \( catppuccin-logo.png -resize 400x400 \) \
  -gravity center -composite \
  catppuccin-latte-wallpaper.png

# Frappé
magick -size 2560x1600 xc:"#303446" \
  \( catppuccin-logo.png -resize 400x400 \) \
  -gravity center -composite \
  catppuccin-frappe-wallpaper.png

# Macchiato
magick -size 2560x1600 xc:"#24273a" \
  \( catppuccin-logo.png -resize 400x400 \) \
  -gravity center -composite \
  catppuccin-macchiato-wallpaper.png

# Mocha (Darkest)
magick -size 2560x1600 xc:"#1e1e2e" \
  \( catppuccin-logo.png -resize 400x400 \) \
  -gravity center -composite \
  catppuccin-mocha-wallpaper.png
```

## Credits

- Logo from [Catppuccin](https://github.com/catppuccin/catppuccin)
- Colors from [Catppuccin Palette](https://catppuccin.com/palette)
