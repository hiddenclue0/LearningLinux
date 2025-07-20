
# 📁 Linux Command Cheat Sheet

This guide shows how to manage files and directories in Linux using simple and advanced commands.

---

## 📂 Copying Files and Directories

| Command                                 | Description                                                                 |
|-----------------------------------------|-----------------------------------------------------------------------------|
| `cp file1.txt file1_copy.txt`           | Copies `file1.txt` to `file1_copy.txt`.                                     |
| `cp file* parent/`                      | Copies all files starting with `file` to the `parent/` directory.           |
| `cp -r parent/ folder1/`                | Copies the entire `parent/` directory and its contents into `folder1/`.     |

## 📄 Moving or Renaming Files and Directories
| Command                                 | Description                                                                 |
|-----------------------------------------|-----------------------------------------------------------------------------|
| `mv file5.txt file55.txt`               | Renames `file5.txt` to `file55.txt`.                                        |
| `mv file5 file55.txt`                   | Moves or renames `file5` to `file55.txt`.                                   |

## 🗑 Removing Files and Directories
| Command                                 | Description                                                                 |
|-----------------------------------------|-----------------------------------------------------------------------------|
| `rm file55.txt`                         | Deletes the `file55.txt` file.                                              |
| `rm f* -r`                              | Recursively deletes all files and directories starting with `f`.            |

> 💡 Be cautious when using `rm -r`, as it permanently deletes files and directories.
## Notes:
- **`-r` option**: Used to operate recursively on directories for `cp` and `rm`.
- **`*` Wildcard**: Matches multiple files or directories following the specified pattern.
- **Warning**: Be cautious with the `rm` command, as it permanently deletes files and directories without recovery.
