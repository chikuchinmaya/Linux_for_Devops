# Linux VM Quick Handbook
## Comprehensive Guide to Linux Administration, Virtualization & DevOps Tools

**Author:** Chinmaya Dalai  
**Connect With Me:**
- LinkedIn: linkedin.com/in/chinmaya-dalai
- GitHub: github.com/chikuchinmaya
- December 2025

---

## Contents

1. Prerequisites for Windows Tools . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 2
   1.1 Installing Chocolatey . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 2
   1.2 Essential Tool Installation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 2

2. Virtual Machine Setup . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 2
   2.1 Manual VM Setup VirtualBox . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 2
   2.2 VM Setup with Vagrant Automated . . . . . . . . . . . . . . . . . . . . . . . . . 2
   2.2.1 Quick Start . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 3
   2.2.2 Vagrant Commands . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 3
   2.2.3 Network Configuration . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 3

3. Linux Fundamentals . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 4
   3.1 Important Linux Directories . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 4
   3.2 Popular Linux Distributions . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 4
   3.2.1 Desktop Linux . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 4
   3.2.2 Server Linux . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 4
   3.3 Basic Linux Commands . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 4
   3.3.1 Path Types . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 4

4. Text Editing with Vim . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 5
   4.1 Installation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 5
   4.2 Opening a File . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 5
   4.3 Vim Modes . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 5
   4.4 Essential Commands . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 5
   4.4.1 Command Mode Navigation . . . . . . . . . . . . . . . . . . . . . . . . . 5
   4.4.2 Extended Mode Colon Commands . . . . . . . . . . . . . . . . . . . . . 5

5. Text Processing Filtering . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 7
   5.1 grep - Search Text . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 7
   5.2 Other Useful Commands . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 7
   5.3 cut and awk . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 7
   5.4 Search and Replace . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 7
   5.4.1 Using Vim . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 7
   5.4.2 Using sed . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 7
   5.5 Piping Redirection . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 8
   5.5.1 Output Redirection . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 8
   5.5.2 Pipes . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 8

6. Finding Files . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 9
   6.1 find Command . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 9
   6.2 locate Command . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 9

7. User and Group Management . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 10
   7.1 Understanding /etc/passwd . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 10
   7.2 User Management Commands . . . . . . . . . . . . . . . . . . . . . . . . . . . . 10

8. File Permissions . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 11
   8.1 Understanding Permissions . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 11
   8.2 Changing Permissions Symbolic . . . . . . . . . . . . . . . . . . . . . . . . . 11
   8.3 Changing Permissions Numeric . . . . . . . . . . . . . . . . . . . . . . . . . . 11
   8.4 Changing Ownership . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 11
   8.4.1 Example Multi-user Access . . . . . . . . . . . . . . . . . . . . . . . . 12

9. Quick Reference Cheatsheet . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 13
   9.1 Directory Navigation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 13
   9.2 File Operations . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 13
   9.3 System Information . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 13

10. System Administration Cheatsheet . . . . . . . . . . . . . . . . . . . . . . . . . . . 14
    10.1 Sudo . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 14
    10.2 Software Management . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 14
    10.3 Services (systemd) . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 15
    10.4 Processes . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 16
    10.5 Archiving . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 16
    10.6 Ubuntu Examples . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 17

---

## 1 Prerequisites for Windows Tools

### 1.1 Installing Chocolatey

Follow the official installation guide at https://chocolatey.org/docs/installation.

### 1.2 Essential Tool Installation

```bash
choco install virtualbox --version 7.1.4 -y
choco install vagrant --version 2.4.3 -y
choco install git -y
choco install corretto17jdk -y
choco install maven -y
choco install awscli -y
choco install intellijidea-community -y
choco install vscode -y
choco install sublimetext3 -y
```

---

## 2 Virtual Machine Setup

### 2.1 Manual VM Setup VirtualBox

1. Enable virtualization (VT-x/AMD-V) in BIOS/UEFI and boot Windows.
2. Open VirtualBox → Click **New** → Provide name → Select OS type.
3. Assign CPU/RAM and disk size as required.
4. Go to **Settings** → **Storage** → Add OS ISO file (CentOS Stream 9 or Ubuntu).
5. Go to **Settings** → **Network** → **Adapter 2** → Enable → Set to **Bridged Adapter**.
6. Select your network adapter (Wi-Fi or Ethernet).
7. **Settings** → **System** → **Pointing Device** → Change to **USB Tablet**.
8. Start VM, complete OS installation, remove ISO, and restart.

**Note:** For Ubuntu, download ISO from https://releases.ubuntu.com/jammy

### 2.2 VM Setup with Vagrant (Automated)

Vagrant simplifies VM creation by reading a **Vagrantfile** and managing VM boxes automatically.

#### 2.2.1 Quick Start

Create directories for VMs:
```bash
mkdir -p vagrant-vms/centos
mkdir -p vagrant-vms/ubuntu
```

Initialize Vagrant with CentOS Stream 9:
```bash
cd vagrant-vms/centos
vagrant init eurolinux-vagrant/centos-stream-9
```

Initialize with Ubuntu 22.04:
```bash
vagrant init ubuntu/jammy64
```

Find available boxes at https://portal.cloud.hashicorp.com/vagrant/discover

#### 2.2.2 Vagrant Commands

| Command | Description |
|---------|-------------|
| `vagrant up` | Start and provision VM |
| `vagrant box list` | List downloaded boxes |
| `vagrant status` | Check VM status |
| `vagrant ssh` | SSH into VM |
| `vagrant halt` | Stop VM |
| `vagrant reload` | Reboot VM with config changes |
| `vagrant destroy` | Delete VM (keeps box) |
| `vagrant global-status` | List all Vagrant environments |

#### 2.2.3 Network Configuration

**Inside Linux VM:**
```bash
ip addr show          # Show all network details
ip a                  # Shortened version
```

**On Windows host:**
```bash
ipconfig              # Show network details
```

---

## 3 Linux Fundamentals

### 3.1 Important Linux Directories

| Directory | Purpose |
|-----------|---------|
| `/root`, `/home/username` | Home directories |
| `/bin`, `/usr/bin`, `/usr/local/bin` | User executables |
| `/media`, `/mnt` | Mount points |
| `/etc` | Configuration files |
| `/tmp` | Temporary files |
| `/boot` | Kernel and bootloader |
| `/var`, `/srv` | Server state data |
| `/proc`, `/sys` | System information |
| `/lib`, `/usr/lib`, `/usr/local/lib` | Shared libraries |

### 3.2 Popular Linux Distributions

#### 3.2.1 Desktop Linux

Ubuntu, Linux Mint, Arch Linux, Fedora, openSUSE, Debian

#### 3.2.2 Server Linux

Red Hat Enterprise Linux, Ubuntu Server, CentOS/AlmaLinux/Rocky, SUSE Linux Enterprise

### 3.3 Basic Linux Commands

#### Essential Commands

| Command | Description |
|---------|-------------|
| `pwd` | Print working directory |
| `mkdir` | Create directory |
| `cd` | Change directory |
| `ls` | List files/directories |
| `touch` | Create empty file |
| `cat` | Show file contents |
| `whoami` | Show current user |
| `uptime` | Show system uptime |
| `free -m` | Memory usage in MB |
| `cat /etc/os-release` | Show OS details |
| `ip addr show` | Show network details |
| `ip a` | Shortened network info |
| `sudo -i` | Become root |
| `sudo su` | Become root (alternative) |

#### 3.3.1 Path Types

- **Absolute Path:** Starts with `/`, complete path from root (e.g., `/home/user/documents`)
- **Relative Path:** Path from current directory (e.g., `./documents` or `..`)

---

## 4 Text Editing with Vim

### 4.1 Installation

```bash
sudo yum install vim -y
```

### 4.2 Opening a File

```bash
vim filename.txt
```

### 4.3 Vim Modes

Vim operates in three modes:

1. **Command (Normal) Mode** - Default mode for navigation and commands.
2. **Insert Mode** - For editing text. Enter with `i`.
3. **Extended (Colon) Mode** - For saving, quitting, searching. Enter with `:`.

### 4.4 Essential Commands

#### 4.4.1 Command Mode Navigation

| Command | Description |
|---------|-------------|
| `gg` | Go to start of file |
| `G` | Go to end of file |
| `w`, `b` | Move forward/backward by word |
| `5w`, `3b` | Move n words forward/backward |
| `u` | Undo last change |
| `Ctrl+r` | Redo changes |
| `yy` | Copy (yank) entire line |
| `nyy` | Copy n lines (e.g., `4yy`) |
| `p` | Paste below cursor |
| `P` | Paste above cursor |
| `dw` | Delete word |
| `x` | Delete character (Backspace-like) |
| `X` | Delete character (Delete-like) |
| `dd` | Delete entire line |
| `ndd` | Delete n lines (e.g., `5dd`) |
| `/pattern` | Search for pattern |

#### 4.4.2 Extended Mode (Colon Commands)

| Command | Description |
|---------|-------------|
| `Esc+w` | Save changes |
| `Esc+q` | Quit without saving |
| `Esc+wq` | Save and quit |
| `Esc+w!` | Save forcefully |
| `Esc+wq!` | Save and quit forcefully |
| `Esc+x` | Save and quit (short form) |
| `Esc+X` | Give password to file |
| `Esc+20n` | Go to line 20 (or any line n) |
| `:set nu` | Set line numbers |
| `:set nonu` | Remove line numbers |

---

## 5 Text Processing & Filtering

### 5.1 grep - Search Text

```bash
grep "root" /etc/passwd              # Find lines with "root"
grep -i "ROOT" /etc/passwd           # Case-insensitive
grep -v "root" /etc/passwd           # Exclude lines with "root"
```

### 5.2 Other Useful Commands

- `less /etc/passwd` - Display file page-wise
- `more /etc/passwd` - Similar to less
- `head /etc/passwd` - Show top 10 lines
- `tail /etc/passwd` - Show last 10 lines

### 5.3 cut and awk

```bash
cut -d: -f1 /etc/passwd              # Extract first field (username)
awk '{print $1}' /etc/passwd         # Print first column
```

### 5.4 Search and Replace

#### 5.4.1 Using Vim

```bash
vim file.txt
:s/old/new/g                         # Replace in current line
:%s/old/new/g                        # Replace in entire file
```

#### 5.4.2 Using sed

```bash
sed 's/tech/tools/g' devopstools     # Replace and display
sed 's/tech/tools/g' devopstools > newtools.txt  # Save to file
```

### 5.5 Piping & Redirection

#### 5.5.1 Output Redirection

| Operator | Description |
|----------|-------------|
| `>` | Overwrite output to file |
| `>>` | Append output to file |
| `2>` | Redirect errors to file |
| `&>` | Redirect all (stdout + stderr) to file |
| `2>/dev/null` | Discard errors |

#### 5.5.2 Pipes

```bash
ls | wc -l                           # Count files
ps aux | grep java                   # Find Java processes
tail /var/log/messages | grep error  # Filter errors from logs
```

---

## 6 Finding Files

### 6.1 find Command

```bash
find /etc -name host                 # Find files named "host"
find /etc -type f -name host         # Find files only (not directories)
find -name "*.conf"                  # Find all config files
find -type d -name logs              # Find all directories named "logs"
find -size +100M                     # Find files larger than 100MB
find -size -10M                      # Find files smaller than 10MB
```

### 6.2 locate Command

```bash
sudo yum install mlocate -y          # Install mlocate
sudo updatedb                        # Update file database
locate filename                      # Search indexed database
```

**Note:** `locate` uses a pre-indexed database, so it's faster than `find` but may show outdated results if `updatedb` hasn't run recently.

---

## 7 User and Group Management

### 7.1 Understanding /etc/passwd

Example entry:
```
root:x:0:0:root:/root:/bin/bash
vagrant:x:1000:1000:vagrant:/home/vagrant:/bin/bash
```

**Format:** `username:password_hash:UID:GID:full_name:home_dir:login_shell`

- **x** - Password stored in `/etc/shadow`
- **UID** - User ID (0 = root)
- **GID** - Group ID

### 7.2 User Management Commands

| Command | Description |
|---------|-------------|
| `useradd username` | Create user (RedHat) |
| `adduser username` | Create user (Ubuntu) |
| `passwd username` | Set/reset password |
| `id username` | Show user info (UID/GID) |
| `su - username` | Switch to user |
| `groupadd groupname` | Create group |
| `usermod -aG groupname username` | Add user to group |
| `userdel -r username` | Remove user with home dir |
| `groupdel groupname` | Remove group |
| `last` | Show last login history |
| `who` | Show logged-in users |
| `whoami` | Show current username |

---

## 8 File Permissions

### 8.1 Understanding Permissions

```
-rwxr-xr-x
| Type | Owner | Group | Others |
|      | rwx   | r-x   | r-x    |
|      | 7     | 5     | 5      |
```

### 8.2 Changing Permissions (Symbolic)

```bash
chmod u+r file                       # Give owner read permission
chmod g-w dir                        # Remove group write permission
chmod o-x dir                        # Remove other execute permission
chmod ugo+r file                     # Give all read permission
```

### 8.3 Changing Permissions (Numeric)

- **4** = Read (r)
- **2** = Write (w)
- **1** = Execute (x)

```bash
chmod 755 myfile                     # rwxr-xr-x
chmod 644 myfile                     # rw-r--r--
chmod 700 mydir                      # rwx------
```

### 8.4 Changing Ownership

```bash
chown user file                      # Change owner
chgrp group file                     # Change group
chown -R user:group directory        # Recursively change owner and group
```

#### 8.4.1 Example Multi-user Access

```bash
chown -R ansible /opt/devops/dir     # Set owner to ansible
chmod 770 /opt/devops/dir            # rwxrwx--- (user + group)
chgrp devops /opt/devops/dir         # Set group to devops
```

---

## 9 Quick Reference Cheatsheet

### 9.1 Directory Navigation

| Command | Description |
|---------|-------------|
| `cd` | Change to home directory |
| `cd -` | Change to previous directory |
| `cd path` | Change to absolute path |
| `cd ./path` | Change to relative path |
| `ls -la` | List all files (including hidden) |

### 9.2 File Operations

| Command | Description |
|---------|-------------|
| `touch file` | Create empty file |
| `rm file` | Delete file |
| `rm -r directory` | Delete directory recursively |
| `cp source dest` | Copy file |
| `cp -r src dest` | Copy directory |
| `mv source dest` | Move/rename file |
| `du -sh directory` | Show directory size |

### 9.3 System Information

| Command | Description |
|---------|-------------|
| `uname -a` | Show system info |
| `uname -m` | Show processor architecture |
| `cat /etc/os-release` | Show OS version |
| `uptime` | Show system uptime |
| `df -h` | Show disk usage |
| `free -m` | Show memory usage in MB |
| `ps aux` | Show running processes |
| `top` | Live process monitor |
| `lsb_release -a` | Show distro info (Ubuntu) |

---

## 10 System Administration Cheatsheet

### 10.1 Sudo

| Command / Entry | Description |
|-----------------|-------------|
| `sudo -i` | Become **root** if user is in sudoers |
| `export EDITOR=vim` | Set vim as default editor for visudo |
| `visudo` | Safely edit `/etc/sudoers` |
| `root ALL=(ALL) ALL` | Root can run any command anywhere |
| `ansibel ALL=(ALL) ALL` | User `ansibel` can run any command with password |
| `ansibel ALL=(ALL) NOPASSWD: ALL` | User `ansibel` can run any command without password |
| `%sudo ALL=(ALL) ALL` | Debian/Ubuntu: all users in `sudo` group have full sudo |
| `/etc/sudoers.d/<file>` | Drop-in sudo rules for users/groups |

### 10.2 Software Management

| Command | Description |
|---------|-------------|
| `cat /etc/os-release` | Show OS details (ID, VERSION, PRETTY_NAME) |
| `rpm -qa` | List installed packages (RPM-based) |
| `dpkg -l` | List installed packages (Debian-based) |
| `rpm -ivh package.rpm` | Install RPM package |
| `dpkg -i package.deb` | Install DEB package |
| `yum install httpd -y` | Install httpd on CentOS/RHEL/Stream |
| `dnf install httpd -y` | Install httpd on CentOS Stream 9 |
| `yum update / dnf update` | Update all packages (RPM-based) |
| `yum remove httpd -y / dnf remove httpd -y` | Remove httpd package |
| `yum repolist / dnf repolist` | List enabled repositories |
| `yum install epel-release` | Enable EPEL repo (YUM) |
| `dnf install epel-release` | Enable EPEL repo (DNF) |
| `yum history / dnf history` | View package transaction history |
| `apt update` | Refresh APT package index |
| `apt install apache2 -y` | Install Apache on Ubuntu |
| `apt remove apache2 -y` | Remove Apache but keep config |
| `apt purge apache2 -y` | Remove Apache and its config |
| `apt search tree` | Search package by name (Ubuntu) |
| `apt show <package>` | Show package details (version, repo, size) |

### 10.3 Services (systemd)

| Command | Description |
|---------|-------------|
| `sudo systemctl start httpd` | Start httpd service (CentOS/RHEL/Stream) |
| `sudo systemctl stop httpd` | Stop httpd service |
| `sudo systemctl restart httpd` | Restart httpd service |
| `sudo systemctl reload httpd` | Reload httpd config without full restart |
| `sudo systemctl status httpd` | Show httpd service status |
| `sudo systemctl enable httpd` | Enable httpd on boot |
| `sudo systemctl disable httpd` | Disable httpd on boot |
| `systemctl is-active httpd` | Check if httpd is running |
| `systemctl is-enabled httpd` | Check if httpd starts at boot |
| `sudo systemctl start apache2` | Start Apache on Ubuntu |
| `sudo systemctl stop apache2` | Stop Apache on Ubuntu |
| `sudo systemctl restart apache2` | Restart Apache on Ubuntu |
| `sudo systemctl reload apache2` | Reload Apache on Ubuntu |
| `sudo systemctl status apache2` | Show Apache status on Ubuntu |
| `systemctl is-active apache2` | Check if Apache is running |
| `systemctl is-enabled apache2` | Check if Apache starts at boot |

### 10.4 Processes

| Command | Description |
|---------|-------------|
| `top` | Live view of CPU/memory and running processes |
| `ps aux` | List all processes with details |
| `ps -ef` | List all processes (full-format) |
| `ps -ef \| grep httpd` | Find processes matching `httpd` |
| `ps -ef \| grep httpd \| grep -v grep` | Filter out the grep process itself |
| `kill <pid>` | Terminate process by PID |
| `kill -9 <pid>` | Force kill process by PID |
| `ps -ef \| grep httpd \| grep -v grep \| awk '{print $2}' \| xargs kill -9` | Kill all httpd processes |

### 10.5 Archiving

| Command | Description |
|---------|-------------|
| `tar -czvf httpd21012025.tar.gz httpd/` | Create compressed tar of `httpd/` directory |
| `tar -xzvf httpd21012025.tar.gz` | Extract tar.gz in current directory |
| `tar -xzvf httpd21012025.tar.gz -C /opt/` | Extract tar.gz into `/opt/` |
| `tar --help` | Show tar help/options |
| `zip -r httpd_210126.zip httpd/` | Create zip archive of `httpd/` directory |
| `unzip httpd_210126.zip` | Extract zip archive |

**Tar options:** `c = create`, `x = extract`, `z = gzip`, `v = verbose`, `f = file`

### 10.6 Ubuntu Examples

| Command | Description |
|---------|-------------|
| `adduser devops` | Create user `devops` on Ubuntu |
| `id devops` | Show UID/GID and groups for `devops` |
| `dpkg -i tree_2.0.2-1_arm64.deb` | Install `tree` from local `.deb` file |
| `apt update && apt install tree` | Update index and install `tree` from repo |
| `dpkg -l \| grep tree` | Verify `tree` package installation |
| `cd /etc/apt && cat sources.list` | View APT repository configuration |
| `apt install apache2` | Install Apache web server |
| `apt remove apache2` | Remove Apache binaries |
| `apt purge apache2` | Remove Apache plus configuration |

---

## Additional Resources

- **Bash Manual:** https://www.gnu.org/software/bash/manual/
- **Vim Official Website:** https://www.vim.org/
- **Vagrant Documentation:** https://www.vagrantup.com/docs
- **VirtualBox:** https://www.virtualbox.org/
- **Chocolatey Package Manager:** https://chocolatey.org/

---

## Author Notes

This handbook is a comprehensive quick reference for Linux system administration, virtualization, and DevOps tools. It covers essential commands, file permissions, user management, practical examples for both beginners and intermediate users, and now includes comprehensive system administration cheatsheets for sudo, software management, services, processes, and archiving.

### For more information and updates, visit:

- **LinkedIn:** https://www.linkedin.com/in/chinmaya-dalai
- **GitHub:** https://github.com/chikuchinmaya

---

**Last Updated:** January 2026
