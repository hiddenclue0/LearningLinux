# 🧭 Basic Navigation Commands in Linux

Mastering directory navigation is essential for working efficiently in the Linux terminal. Here are the most common commands to help you move around and inspect your file system.

---

## 📁 Directory Navigation

| Command      | Description                                                                 |
|--------------|-----------------------------------------------------------------------------|
| `pwd`        | Print the **current working directory** (shows where you are).              |
| `cd`         | Change directory. Without arguments, it goes to your home directory.        |
| `cd ..`      | Move **one level up** in the directory tree.                                |
| `cd ~`       | Shortcut to move to the **home directory**.                                 |
| `cd -`       | Switch to the **previous directory** you were in.                           |

---

## 📂 Listing Files & Directories

| Command        | Description                                                                          |
|----------------|--------------------------------------------------------------------------------------|
| `ls`           | List files and folders in the current directory.                                     |
| `ls -a`        | Lists **all files**, including hidden ones (those starting with `.`).                |
| `ls -l`        | Long listing format: shows **permissions, owners, size, timestamps**.                |
| `ls -la`       | Combines `-l` and `-a`: shows all files with detailed info.                          |
| `ls /var`      | Lists contents of the `/var` directory.                                              |
| `ls /var -la`  | Lists `/var` directory contents in long format including hidden files.               |
| `ll`           | Alias for `ls -l` on many Linux systems (depends on shell config).                   |

---

> 💡 Tip: Combine flags like `ls -lah` to include hidden files and human-readable sizes.

---

## ✅ Practice Example

```bash
cd ~            # Go to home directory
pwd             # Confirm your location
cd /var/log     # Go into /var/log
ls -la          # List all contents in long format
cd -            # Jump back to previous location
