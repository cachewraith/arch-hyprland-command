# 🎨 Custom Tools & Eye Candy

You have built-in tools for customizing your Hyprland environment.

### **1. Wallpaper Management**
- `setwall <image_url>`: Your custom function for setting high-resolution wallpapers.
  - It downloads the image to your `~/Downloads/`.
  - It automatically applies it using your wallpaper engine.
  - It caches the image for Hyprland to use.
- **Example**: `setwall https://example.com/cool-image.jpg`

### **2. Minecraft & Performance**
- `mc <launcher>`: Launches your game using **GameMode**.
- `minecraft`: A direct shortcut for your launcher with performance optimizations.
- **NVIDIA Boost**: I've enabled `__GL_THREADED_OPTIMIZATIONS=1` in your system, so any OpenGL app like Minecraft will automatically run with better multi-threading.

### **3. Prompt & Style**
- Your terminal uses **Starship**, a modern prompt that shows your current folder, Git status, and command execution time.
- If you change your `.bashrc`, always run `src` to see the updates!
