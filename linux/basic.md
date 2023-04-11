---
id: "basic"
aliases:
  - "Install package"
tags:
  - "linux"
---

<!--toc:start-->
- [Install package](#install-package)
  - [For .deb](#for-deb)
  - [For .AppImage](#for-appimage)
- [Fix package](#fix-package)
<!--toc:end-->

# Install package
## For .deb
```bash
sudo dpkg -i *.deb
```
## For .AppImage
```bash
chmod +777 *.AppImage
./*.AppImage
```

# Fix package
```bash
sudo apt -f install
sudo apt update
sudo apt install [dependencies]
...
sudo apt install [package]
```

# Manage process
See all the process:
```bash
ps aux
```
Find the target pid
 ```bash
pgrep [partial name] 
 ```
 return the pid of the process
 kill the process
 ```bash
kill [pid]
 ```

