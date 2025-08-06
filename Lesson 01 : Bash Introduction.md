
# 🚀 Bash Introduction 

## 🔹 What is Bash?

* **Bash** = **Bourne Again SHell**
* It’s a **command-line interpreter** (shell) in Linux/Unix.
* Used to **execute commands**, **write scripts**, and **control the system**.

---

## 🔹 Basic Bash Syntax

```
command [options] [arguments]
```

* **command** → What you want to run (e.g., ls, cd)
* **options** → Modify the command’s behavior (e.g., -l, -a)
* **arguments** → The target of the command (e.g., file name, directory)

---

## 🔹 Essential Bash Commands

| Command       | Meaning                         |
| ------------- | ------------------------------- |
| `pwd`         | Print current working directory |
| `ls`          | List files in directory         |
| `cd`          | Change directory                |
| `mkdir`       | Create a new directory          |
| `rmdir`       | Remove empty directory          |
| `touch file`  | Create a new empty file         |
| `cat file`    | Show file content               |
| `cp src dest` | Copy file/directory             |
| `mv src dest` | Move/Rename file                |
| `rm file`     | Remove file                     |
| `clear`       | Clear terminal screen           |
| `history`     | Show command history            |

---

## 🔹 File Permissions (Shortcut)

```
ls -l
```

Output like:

```
-rwxr-xr--  1 user group size date filename
```

* **r = read, w = write, x = execute**
* Change permissions:

```
chmod 755 file
```

---

## 🔹 Bash Operators

* **Redirection** → `>` (output), `>>` (append), `<` (input)
* **Pipe** → `|` (send output of one command to another)
* **Background** → `&` (run in background)
* **Logical** → `&&` (AND), `||` (OR)

---

## 🔹 Bash Shortcuts

| Shortcut   | Action                             |
| ---------- | ---------------------------------- |
| `Ctrl + C` | Stop a command                     |
| `Ctrl + Z` | Pause/stop and put in background   |
| `Ctrl + D` | Logout/exit shell                  |
| `!!`       | Repeat last command                |
| `!abc`     | Run last command starting with abc |
| `Tab`      | Auto-complete command/file         |
| `↑ / ↓`    | Scroll through command history     |
| `Ctrl + L` | Clear screen (like `clear`)        |

---

## 🔹 Bash Script Structure

```bash
#!/bin/bash
# My first script

echo "Hello, World!"
```

Run script:

```
chmod +x script.sh
./script.sh
```