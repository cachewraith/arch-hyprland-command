# 🚀 System Navigation (Your Arch Setup)

You have several shortcuts (aliases) to move around your folders quickly.

### **1. Fast Navigation (Zoxide)**
Your `cd` command is actually using **Zoxide**, which "remembers" where you've been.
- `cd <folder_name>`: Jump to any folder you've visited before, even if you aren't in the parent directory.
- `zi`: Opens an interactive list of your most visited folders. Use arrow keys to select and press **Enter**.

### **2. Listing Files (Eza)**
Instead of the standard `ls`, you are using `eza`, which is colorful and shows icons.
- `ls`: Shows a tree view of the current folder (Level 1).
- `la`: Shows all files, including hidden ones (starting with `.`).
- `ll`: Long format. Shows file sizes and permissions (but hides the time for a cleaner look).
- `tree`: Shows a deep tree view of all subfolders (Level 3).

### **3. Jumping Back**
- `..`: Go back one folder.
- `...`: Go back two folders.
- `.`: Go straight to the root directory (`/`).

### **4. System Commands**
- `src`: Reloads your configuration. Use this after you change your `.bashrc` or aliases.
- `clr` or `c`: Clears the screen.
- `q`: Exits the terminal.
