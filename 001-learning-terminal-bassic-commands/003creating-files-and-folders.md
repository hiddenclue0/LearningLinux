# 📁 Creating Files and Folders in Linux

This guide shows how to create directories and files using simple and advanced commands.

---

## 📂 Creating Directories

| Command                                 | Description                                                                 |
|-----------------------------------------|-----------------------------------------------------------------------------|
| `mkdir linux`                           | Creates a directory named `linux` in the current path.                      |
| `mkdir folder1 folder2 folder3 folder4`| Creates **multiple directories** at once.                                   |
| `mkdir Folder1`                         | Creates `Folder1`. Case-sensitive, so it's different from `folder1`.        |
| `mkdir -p parent/child/grandChild`      | Creates a **nested directory structure**. Creates all missing parent dirs.  |
| `tree`                                  | Shows a visual tree of directories (requires `tree` package).               |

### 🌳 Example Output of `tree`

```bash
.
└── parent
    └── child
        └── grandChild

3 directories, 0 files
```


> 💡 Use `-p` to avoid "No such file or directory" when making nested folders.

---

## 📄 Creating Files

| Command                 | Description                                                              |
|-------------------------|--------------------------------------------------------------------------|
| `touch text.txt`        | Creates an empty file named `text.txt`.                                 |
| `touch file{1..5}`      | Creates multiple files: `file1`, `file2`, ..., `file5`.                  |
| `echo > newfile10.txt`  | Creates `newfile10.txt` or clears it if it exists (writes nothing).      |
| `cat > newfile11.txt`   | Opens prompt to write content into the file. Press `Ctrl + D` to save.   |

### ✍️ Example: Writing to a File
```bash
cat > newfile11.txt
1
2
3
4
5
# Press Ctrl + D here to save
