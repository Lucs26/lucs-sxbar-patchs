# lucs-sxbar-patchs

A patch that adds custom modules to sxbar.

**Note**: This is a community patch and not officially affiliated with the sxbar project.

## 📦 Requirements

- [sxbar](https://github.com/uint23/sxbar) source code
- `patch` utility
- Build tools

## 📖 Patch Details

This patch modifies and extends sxbar with the following modules:

### 🔧 Modified Original Modules
- **CPU** (%) 
- **Volume** (%) 
- **Time** (HH:MM:SS)
- **Date** (YY-MM-DD)

### 🆕 New Custom Modules
- **RAM** (used Mi / total Gi)
- **Disk** (%) 
- **Network Connection** (|NET-OK| or ---)

## 🚀 Quick Install
```bash
# Clone sxbar (if you haven't already)
git clone https://github.com/uint23/sxbar
# Clone this repository 
git clone https://github.com/Lucs26/lucs-sxbar-patchs

# Copy and apply the patch
cp lucs-sxbar-patchs/modules.patch sxbar/
cd sxbar
patch -p1 < modules.patch

# Install
sudo make install
