# linux-commands-guide
A comprehensive guide to Linux commands and file system for beginners and intermediate users.


# Linux Commands & File System Guide 

This repository is a beginner-friendly guide to essential Linux commands and the file system structure.

---

## 📂 Linux File System Hierarchy

| Directory | Purpose |
|-----------|---------|
| `/`       | Root directory – everything starts here |
| `/home`   | Personal folders for users |
| `/etc`    | System configuration files |
| `/var`    | Variable data (logs, caches) |
| `/tmp`    | Temporary files (deleted on reboot) |
| `/bin`    | Essential executable programs |

---

## 🔥 Essential Linux Commands

### File & Directory Operations
```bash
ls              # List contents of current directory
ls -la          # Show all files (including hidden) with details
cd /home        # Change directory
pwd             # Show current path
mkdir myfolder  # Create a new folder
rm file.txt     # Delete a file
rm -rf folder/  # Force delete a folder and its contents
cp source dest  # Copy a file
mv old new      # Move or rename a file

##Viewer and editing file 
cat file.txt    # Display entire file
less file.txt   # View file page by page (press 'q' to exit)
head -10 file   # Show first 10 lines
tail -20 file   # Show last 20 lines
nano file.txt   # Edit using Nano editor
vim file.txt    # Edit using Vim editor

##Permission management 
chmod 755 script.sh  # Set read/write/execute permissions
chown user:group file # Change file owner/group

##Networking Commands
ping google.com  # Test network connection
curl ifconfig.me # Get public IP address
ssh user@ip      # Log into a remote server via SSH

##Process and system monitoring 
ps aux          # Show all running processes
top             # Real-time system monitor
kill PID        # Stop a process by its ID
df -h           # Show disk space (human-readable)
du -sh folder/  # Show folder size

##Practical Example 
mkdir ~/project
cd ~/project
echo '#!/bin/bash' > hello.sh
echo 'echo "Hello Linux"' >> hello.sh
chmod +x hello.sh
./hello.sh







এই রিপোজিটরি Linux-এর কমান্ড এবং ফাইল সিস্টেম স্ট্রাকচার শেখার জন্য তৈরি। নতুন ইউজারদের জন্য সহজ ভাষায় ব্যাখ্যা দেওয়া হয়েছে।

## 📂 Linux File System Hierarchy
Linux-এর ফাইল সিস্টেম একটি **ট্রি স্ট্রাকচার**:

| ডিরেক্টরি | ব্যবহার |
|-----------|---------|
| `/` | রুট ডিরেক্টরি (সবকিছুর শুরু) |
| `/home` | সাধারণ ইউজারদের ফোল্ডার |
| `/etc` | কনফিগারেশন ফাইল |
| `/var` | পরিবর্তনশীল ডেটা (লগ, ক্যাশে) |
| `/tmp` | অস্থায়ী ফাইল (রিবুটে মুছে যায়) |
| `/bin` | প্রয়োজনীয় এক্সিকিউটেবল প্রোগ্রাম |

---

## 🔥 প্রয়োজনীয় Linux কমান্ড (বাংলায় ব্যাখ্যা)

### 1. ফাইল ও ডিরেক্টরি নিয়ে কাজ
```bash
ls              # বর্তমান ডিরেক্টরির কন্টেন্ট দেখায়
ls -la          # সব ফাইল (লুকানো সহ) বিস্তারিত দেখায়
cd /home        # নির্দিষ্ট ডিরেক্টরিতে যান
pwd             # বর্তমান পাথ দেখায়
mkdir myfolder  # নতুন ফোল্ডার তৈরি
 
rm file.txt     # ফাইল ডিলিট করে
rm -rf folder/  # ফোল্ডার ও সব কন্টেন্ট ফোর্স ডিলিট
cp source dest  # ফাইল কপি
mv old new      # ফাইল মুভ বা রিনেম

cat file.txt    # পুরো ফাইল দেখায়
less file.txt   # পেজ আকারে
head -10 file   # প্রথম ১০ লাইন
tail -20 file   # শেষ ২০ লাইন
nano file.txt   # এডিট

chmod 755 script.sh  # পারমিশন সেট
chown user:group file # মালিকানা পরিবর্তন

ps aux          # চলমান প্রক্রিয়া
top             # রিয়েল-টাইম মনিটর
kill PID        # প্রক্রিয়া বন্ধ
df -h           # ডিস্ক স্পেস
du -sh folder/  # ফোল্ডার সাইজ


ping google.com  # কানেকশন টেস্ট
curl ifconfig.me # পাবলিক IP
ssh user@ip      # রিমোট লগইন


