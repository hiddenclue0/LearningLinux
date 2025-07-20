
# 👁️ Viewing Files (Linux)

This cheat sheet contains various Linux commands to view and navigate files efficiently in the terminal.

---

## 📄 Using `more` to View Files

| Command                                 | Description                                                                 |
|-----------------------------------------|-----------------------------------------------------------------------------|
| `more 120 remo_poem.txt`                | Displays the first 120 lines of `remo_poem.txt`.                            |
| `ls`                                    | Lists the contents of the current directory.                                |
| `more -120 remo_poem.txt`               | Displays the last 120 lines of `remo_poem.txt`.                             |
| `more -120 5 remo_poem.txt`             | Starts displaying from line 120 to line 5 in `remo_poem.txt`.               |
| `more -5 +/Remo remo_poem.txt`         | Displays lines starting from the pattern `/Remo` in `remo_poem.txt`.        |
| `more -s remo_poem.txt`                | Collapses multiple empty lines into one when displaying `remo_poem.txt`.    |

### 🌳 Example: Using `more` to View and Search

```bash
$ more 120 remo_poem.txt
$ more -5 +/Remo remo_poem.txt
```

---

## 📄 Using `less` to View Files

| Command                                 | Description                                                                 |
|-----------------------------------------|-----------------------------------------------------------------------------|
| `less remo_poem.txt`                    | Opens `remo_poem.txt` for scrolling and viewing.                             |
| `less -p remo_poem.txt`                 | Highlights the first occurrence of `remo_poem.txt` in the file.             |
| `less -p "Remo" remo_poem.txt`         | Highlights the first occurrence of the word "Remo" in the file.             |
| `less -p "Romeo" remo_poem.txt`        | Highlights the first occurrence of the word "Romeo" in the file.            |
| `less -NIp "Romeo" remo_poem.txt`      | Case-insensitive search for the word "Romeo", with highlighting.           |
| `less -NIp "Romeo" remo_poem.txt`      | Case-insensitive, highlighting "Romeo" in `remo_poem.txt`.                  |

### 🌳 Example: Using `less` to View and Search

```bash
$ less remo_poem.txt
$ less -p "Romeo" remo_poem.txt
$ less -NIp "Romeo" remo_poem.txt
```

---

## 📄 Using `head` to View the Start of Files

| Command                                 | Description                                                                 |
|-----------------------------------------|-----------------------------------------------------------------------------|
| `head remo_poem.txt`                    | Displays the first 10 lines of `remo_poem.txt`.                             |
| `head -140 remo_poem.txt`               | Displays the first 140 lines of `remo_poem.txt`.                            |
| `head -c 10 remo_poem.txt`              | Displays the first 10 bytes of `remo_poem.txt`.                             |

### 🌳 Example: Using `head` to View the Start of Files

```bash
$ head remo_poem.txt
$ head -c 10 remo_poem.txt
```

---

## 📄 Using `tail` to View the End of Files

| Command                                 | Description                                                                 |
|-----------------------------------------|-----------------------------------------------------------------------------|
| `tail remo_poem.txt`                    | Displays the last 10 lines of `remo_poem.txt`.                              |
| `tail -50 remo_poem.txt`                | Displays the last 50 lines of `remo_poem.txt`.                              |
| `tail -c 50 remo_poem.txt`              | Displays the last 50 bytes of `remo_poem.txt`.                              |

### 🌳 Example: Using `tail` to View the End of Files

```bash
$ tail remo_poem.txt
$ tail -c 50 remo_poem.txt
```

---

## Notes:
- **`more` and `less`**: Useful for viewing large files in chunks, allowing scrolling and searching.
- **`head` and `tail`**: Useful for quickly viewing the beginning or end of a file.
- **`-p` and `-s` options**: Customize how `less` and `more` behave during file navigation.
