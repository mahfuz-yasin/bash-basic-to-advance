
# ⚙️ Setting Up Bash

## 🔹 Step 1: Check if Bash is Installed

Most Linux & macOS systems come with Bash preinstalled.
Run:

```bash
bash --version
```

If you see version info → ✅ Bash is installed.
If not, install it (next step).

---

## 🔹 Step 2: Install Bash

### On Ubuntu/Debian

```bash
sudo apt update
sudo apt install bash
```

### On Fedora/CentOS/RHEL

```bash
sudo dnf install bash
```

or

```bash
sudo yum install bash
```

### On macOS

* Bash is already included.
* For latest version:

```bash
brew install bash
```

(Requires **Homebrew**)

### On Windows

Option 1: **Git Bash**

* Download & install [Git for Windows](https://git-scm.com/).
* Open **Git Bash** for Bash commands.

Option 2: **WSL (Windows Subsystem for Linux)**

```powershell
wsl --install
```

* Restart computer, then run:

```bash
wsl
```

---

## 🔹 Step 3: Start Bash

* Linux/macOS: Open **Terminal** → type:

```bash
bash
```

* Windows:

  * If using Git Bash: just open **Git Bash** app.
  * If using WSL: open **PowerShell** → run:

```powershell
wsl
```

---

## 🔹 Step 4: Set Bash as Default Shell

### On Linux/macOS

```bash
chsh -s /bin/bash
```

(You may need to log out and back in.)

### On WSL (Windows)

* Bash is default when you start WSL.

---

## 🔹 Step 5: Customize Bash (Optional but Recommended)

1. **Edit .bashrc** file (user configuration):

```bash
nano ~/.bashrc
```

2. Add aliases, prompt settings, etc. Example:

```bash
alias ll='ls -la'
PS1="\u@\h:\w\$ "
```

3. Apply changes:

```bash
source ~/.bashrc
```

---

## 🔹 Step 6: Create First Bash Script

```bash
nano hello.sh
```

Paste:

```bash
#!/bin/bash
echo "Hello from Bash!"
```

Make it executable:

```bash
chmod +x hello.sh
./hello.sh
```
