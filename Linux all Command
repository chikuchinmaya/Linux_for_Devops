# Linux & DevOps Complete Command Reference

---

## 1. Windows Prerequisites (Chocolatey)

| Command | Description |
|--------|------------|
| `choco install virtualbox --version 7.1.4 -y` | Install VirtualBox |
| `choco install vagrant --version 2.4.3 -y` | Install Vagrant |
| `choco install git -y` | Install Git |
| `choco install corretto17jdk -y` | Install Amazon Corretto JDK 17 |
| `choco install maven -y` | Install Maven |
| `choco install awscli -y` | Install AWS CLI |
| `choco install intellijidea-community -y` | Install IntelliJ IDEA Community |
| `choco install vscode -y` | Install Visual Studio Code |
| `choco install sublimetext3 -y` | Install Sublime Text |

---

## 2. Virtual Machine Setup (Vagrant)

| Command | Description |
|--------|------------|
| `mkdir -p vagrant-vms/centos` | Create CentOS VM directory |
| `mkdir -p vagrant-vms/ubuntu` | Create Ubuntu VM directory |
| `cd vagrant-vms/centos` | Change directory |
| `vagrant init eurolinux-vagrant/centos-stream-9` | Initialize CentOS VM |
| `vagrant init ubuntu/jammy64` | Initialize Ubuntu VM |
| `vagrant up` | Start VM |
| `vagrant box list` | List Vagrant boxes |
| `vagrant status` | VM status |
| `vagrant ssh` | SSH into VM |
| `vagrant halt` | Stop VM |
| `vagrant reload` | Restart VM |
| `vagrant destroy` | Delete VM |
| `vagrant global-status` | Show all Vagrant VMs |
| `ip addr show` | Show Linux IP addresses |
| `ip a` | Short IP command |
| `ipconfig` | Show Windows IP info |

---

## 3. Linux Fundamentals

| Command | Description |
|--------|------------|
| `pwd` | Print working directory |
| `mkdir` | Create directory |
| `cd` | Change directory |
| `ls` | List files |
| `touch` | Create empty file |
| `cat` | View file content |
| `whoami` | Current user |
| `uptime` | System uptime |
| `free -m` | Memory usage |
| `cat /etc/os-release` | OS information |
| `ip addr show` | Show network info |
| `ip a` | Short network info |
| `sudo -i` | Root login shell |
| `sudo su` | Switch to superuser |

---

## 4. Text Editing with Vim

| Command | Description |
|--------|------------|
| `sudo yum install vim -y` | Install Vim |
| `vim filename.txt` | Open file |
| `gg` | Go to top |
| `G` | Go to bottom |
| `w` | Move word forward |
| `b` | Move word backward |
| `5w` | Move 5 words forward |
| `3b` | Move 3 words backward |
| `u` | Undo |
| `Ctrl+r` | Redo |
| `yy` | Copy line |
| `4yy` | Copy 4 lines |
| `p` | Paste after |
| `P` | Paste before |
| `dw` | Delete word |
| `x` | Delete character |
| `X` | Delete character backward |
| `dd` | Delete line |
| `5dd` | Delete 5 lines |
| `/pattern` | Search text |
| `:w` | Save file |
| `:q` | Quit Vim |
| `:wq` | Save and quit |
| `:w!` | Force save |
| `:wq!` | Force save and quit |
| `:x` | Save and exit |
| `:X` | Save and exit |
| `:20` | Go to line 20 |
| `:set nu` | Show line numbers |
| `:set nonu` | Hide line numbers |

---

## 5. Text Processing & Filtering

| Command | Description |
|--------|------------|
| `grep "root" /etc/passwd` | Search text |
| `grep -i "ROOT" /etc/passwd` | Case-insensitive search |
| `grep -v "root" /etc/passwd` | Exclude lines |
| `less /etc/passwd` | View file page-wise |
| `more /etc/passwd` | View file |
| `head /etc/passwd` | First lines |
| `tail /etc/passwd` | Last lines |
| `cut -d: -f1 /etc/passwd` | Extract first column |
| `awk '{print $1}' /etc/passwd` | Print first field |
| `vim file.txt` | Open file |
| `:s/old/new/g` | Replace text in line |
| `:%s/old/new/g` | Replace text in file |
| `sed 's/tech/tools/g' devopstools` | Replace text |
| `sed 's/tech/tools/g' devopstools > newtools.txt` | Redirect output |
| `ls \| wc -l` | Count files |
| `ps aux \| grep java` | Search Java process |
| `tail /var/log/messages \| grep error` | Filter logs |

---

## 6. Finding Files

| Command | Description |
|--------|------------|
| `find /etc -name host` | Find file by name |
| `find /etc -type f -name host` | Find file only |
| `find -name "*.conf"` | Find config files |
| `find -type d -name logs` | Find directories |
| `find -size +100M` | Files > 100MB |
| `find -size -10M` | Files < 10MB |
| `sudo yum install mlocate -y` | Install locate |
| `sudo updatedb` | Update locate DB |
| `locate filename` | Find file quickly |

---

## 7. User and Group Management

| Command | Description |
|--------|------------|
| `useradd username` | Add user |
| `adduser username` | Add user (interactive) |
| `passwd username` | Set password |
| `id username` | User details |
| `su - username` | Switch user |
| `groupadd groupname` | Add group |
| `usermod -aG groupname username` | Add user to group |
| `userdel -r username` | Delete user |
| `groupdel groupname` | Delete group |
| `last` | Login history |
| `who` | Logged-in users |
| `whoami` | Current user |

---

## 8. File Permissions

| Command | Description |
|--------|------------|
| `chmod u+r file` | Add read to user |
| `chmod g-w dir` | Remove write from group |
| `chmod o-x dir` | Remove execute from others |
| `chmod ugo+r file` | Add read to all |
| `chmod 755 myfile` | rwxr-xr-x |
| `chmod 644 myfile` | rw-r--r-- |
| `chmod 700 mydir` | Owner only |
| `chown user file` | Change owner |
| `chgrp group file` | Change group |
| `chown -R user:group directory` | Recursive ownership |
| `chown -R ansible /opt/devops/dir` | Change owner recursively |
| `chmod 770 /opt/devops/dir` | Full access owner/group |
| `chgrp devops /opt/devops/dir` | Change group |

---

## 9. Quick Reference Cheatsheet

| Command | Description |
|--------|------------|
| `cd` | Change directory |
| `cd -` | Previous directory |
| `cd path` | Change to path |
| `cd ./path` | Relative path |
| `ls -la` | Detailed list |
| `touch file` | Create file |
| `rm file` | Delete file |
| `rm -r directory` | Delete directory |
| `cp source dest` | Copy file |
| `cp -r src dest` | Copy directory |
| `mv source dest` | Move/Rename |
| `du -sh directory` | Directory size |
| `uname -a` | Kernel info |
| `uname -m` | Architecture |
| `cat /etc/os-release` | OS info |
| `uptime` | System uptime |
| `df -h` | Disk usage |
| `free -m` | Memory usage |
| `ps aux` | Process list |
| `top` | Process monitor |
| `lsb_release -a` | Distro info |

---

## 10. System Administration

### 10.1 Sudo

| Command | Description |
|--------|------------|
| `sudo -i` | Root shell |
| `export EDITOR=vim` | Set default editor |
| `visudo` | Edit sudoers safely |

### 10.2 Software Management

| Command | Description |
|--------|------------|
| `cat /etc/os-release` | OS details |
| `rpm -qa` | List RPM packages |
| `dpkg -l` | List DEB packages |
| `rpm -ivh package.rpm` | Install RPM |
| `dpkg -i package.deb` | Install DEB |
| `yum install httpd -y` | Install Apache |
| `dnf install httpd -y` | Install Apache (DNF) |
| `yum update` | Update system |
| `dnf update` | Update system |
| `yum remove httpd -y` | Remove Apache |
| `dnf remove httpd -y` | Remove Apache |
| `yum repolist` | List repos |
| `dnf repolist` | List repos |
| `yum install epel-release` | Enable EPEL |
| `dnf install epel-release` | Enable EPEL |
| `yum history` | Yum history |
| `dnf history` | DNF history |
| `apt update` | Update APT |
| `apt upgrade` | Upgrade packages |
