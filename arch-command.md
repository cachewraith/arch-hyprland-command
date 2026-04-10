# Arch Linux & Hyprland Command Reference

This document covers essential commands for managing your desktop environment, focusing on the custom wallpaper system we've set up.

## 🖼️ Wallpaper Management

### 1. New Custom Command: `setwall`
We added this function to your `~/.bash/functions.sh` to allow downloading and setting any high-resolution image from the web.

**Usage:**
```bash
setwall <IMAGE_URL>
```
```bash
setwall <path to file>
```
**Set icon terminal**
```bash
setanime <path to image.png>
```

**What it does:**
*   **Downloads** the image to `~/Downloads/wallpaper_YYYYMMDD_HHMMSS.ext`.
*   **Unique Filenames:** Uses timestamps so you don't overwrite your previous 4K/8K downloads.
*   **Sets Wallpaper:** Uses `awww` with a "grow" transition effect.
*   **Updates System Cache:** Automatically links the image to `~/.config/hypr/.cache/current_wallpaper.png` so your **Lockscreen** and other scripts stay in sync.
*   **Resolution Check:** If `ImageMagick` is installed, it will tell you the exact resolution (e.g., 3840x2160 for 4K).

---

### 2. Built-in Hyprland Wallpaper Commands
Your system uses the **`awww`** engine.

*   **Set a local file manually:**
    ```bash
    awww img /path/to/image.png
    ```
*   **Change to a random wallpaper (themed):**
    ```bash
    ~/.config/hypr/scripts/Wallpaper.sh
    ```
*   **Open Wallpaper Selector UI:**
    ```bash
    ~/.config/hypr/scripts/WallpaperSelect.sh
    ```

---

## ⌨️ Keyboard Shortcuts (Hyprland)

| Shortcut | Action |
| :--- | :--- |
| `Super + W` | Change to a random wallpaper from your current theme. |
| `Super + Shift + W` | Open the wallpaper selection menu. |
| `Super + Alt + E` | Switch wallpaper engine (awww/hyprpaper). |

---

## 📂 Important Directories

*   **Wallpapers Folder:** `~/.config/hypr/Wallpapers/` (Organized by theme: Catppuccin, Gruvbox, etc.)
*   **Wallpaper Cache:** `~/.config/hypr/.cache/` (Where `current_wallpaper.png` is stored for the lockscreen).
*   **Bash Config:** `~/.bash/functions.sh` (Where the `setwall` code lives).

---

## 🔧 System Tips for 4K/8K
*   **Direct Links:** Always use the "Direct Link" (ending in .jpg or .png) from sites like Wallhaven or Unsplash.
*   **Lockscreen Compatibility:** Your lockscreen (`hyprlock`) currently only supports `.png` for the background. If you set a `.jpg` as your wallpaper, the lockscreen may not show it unless you convert it to PNG in the cache folder.
