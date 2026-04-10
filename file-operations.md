# 📄 File Operations & Searching

You have advanced tools like `bat` and `fzf` installed to help you find and read files faster.

### **1. Reading Files (Bat)**
Your `cat` command is aliased to `bat`.
- `cat <filename>`: Shows the file content with line numbers, syntax highlighting, and Git changes.
- It automatically handles long files by letting you scroll. Press **q** to exit.

### **2. Finding Files (FZF)**
You have a very powerful search alias called `find`.
- `find`: Type this to open an interactive search.
- **Type anything**: It will fuzzy-search through all files in your current folder.
- **Preview**: You will see a preview of the file on the right side.
- **Open**: Press **Enter** to immediately open the selected file in `nvim` (Neovim).

### **3. Copying & Deleting**
You have custom functions to make these safer:
- `cp`: Uses your custom `fn_copy_paste` function.
- `rmv <file>`: Removes a file or directory (one at a time).
- `srm <file>`: **Danger!** Forcefully removes a file using `sudo rm -rf`. Use this only if you are sure.

### **4. Editing**
- `open`: Opens the current folder in `nvim`.
- `snv`: Opens a file in `nvim` with `sudo` (root) permissions.
