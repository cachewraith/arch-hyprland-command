# 🛠️ System Maintenance & Hardware

These commands help you check your system's health and keep it running fast.

### **1. Package Management**
- `sudo pacman -S <package_name>`: Install a new package.
- `sudo pacman -Syu`: Update all your software (do this often!).
- `sudo pacman -Rns <package_name>`: Completely remove a package and its settings.

### **2. Checking Resources**
- `mem`: Shows your current memory (RAM) usage.
- `disk`: Shows your free disk space.
- `fastfetch`: Shows your system information, hardware, and uptime in a cool logo.

### **3. Boot & Grub**
- `grubup`: Updates your bootloader (Grub) configuration. Run this after you change themes or boot settings.

### **4. Performance Tuning**
- `powerprofilesctl set performance`: Forces the system into "High Performance" mode.
- `powerprofilesctl set balanced`: Switches back to normal power usage.
- `gamemoderun <command>`: Runs any app or game with maximum system priority.
