# Understanding Linux File System

## Linux Terminal Structure

Example:

```bash
erabh@Abhi:/mnt/c/Users/erabh/Shell-Master$
```

### Understanding This

| Part | Meaning |
|---|---|
| `erabh` | Username |
| `@` | Separator |
| `Abhi` | Hostname |
| `:` | Separator |
| `/mnt/c/Users/erabh/Shell-Master` | Present Working Directory |
| `$` | Normal User |

---

# Important Symbols

## `/` (Root Directory)

This is the root directory.

Everything in Linux starts from `/`.

All files and folders are stored inside this root path.

---

## `~` (Home Directory)

`~` represents the home directory of the current user.

Example:

```bash
cd ~
```

---

# LS Command

```bash
ls
```

Used to list files and directories.

---

# Root User Access

To switch to root user:

```bash
sudo su -
```

## SUDO

`sudo` means:

```text
Super User Do
```

Used for administrative access.

---

# Binary Files

Binary files are executable command files.

Examples:

- ls
- grep
- cp
- mv

---

# Linux Root Folders

## Folder 1 → `/sbin`

```bash
/sbin -> /usr/sbin
```

These are system binaries or system commands used to manage the Linux system.

Mostly used by administrators.

Examples:
- reboot
- shutdown
- fdisk

---

## Folder 2 → `/lib`

```bash
/lib -> /usr/lib
```

These are system libraries required by commands and applications.

---

## Folder 3 → `/boot`

Used during Linux startup or restart.

Contains:
- Bootloader files
- Kernel files

---

## Folder 4 → `/bin`

```bash
/bin -> /usr/bin
```

`bin` stands for:

```text
Binary
```

These are normal user command binaries.

Examples:
- ls
- cat
- pwd
- mkdir

---

## Folder 5 → `/usr`

Contains files for both:
- Administrative users
- Non-administrative users

Stores:
- Applications
- Libraries
- Utilities
- Documentation

---

## Folder 6 → `/srv`

Server folder.

Used to store:
- Server data
- Server configurations

---

## Folder 7 → `/opt`

Used for third-party or custom tools.

If we install custom software, we usually create a directory inside `/opt`.

Central location for:
- Third-party tools
- Custom applications

---

## Folder 8 → `/mnt`

Mount directory.

Used to:
- Mount temporary storage
- Attach new volumes
- Access external storage

---

## Folder 9 → `/var`

Stores variable data.

Mainly used for:
- Log files
- Cache
- Application data

Important location:

```bash
/var/log
```

Web server logs are usually stored here.

---

## Folder 10 → `/home`

Used to create and store normal user directories.

Example:

```bash
/home/abhi
```

---

## Folder 11 → `/proc`

Virtual file system.

Stores:
- Process information
- Kernel information
- System runtime information

---

## Folder 12 → `/tmp`

Stores temporary files.

These files may get deleted automatically after reboot.

---

## Folder 13 → `/root`

Home directory of the root user.

---

## Folder 14 → `/run`

Stores runtime process data while the system is running.

---

## Folder 15 → `/etc`

Most important Linux directory.

Stores all Linux system configuration files.

Examples:

```bash
/etc/passwd
/etc/ssh/
/etc/hostname
```

---

# PATH Variable

Command:

```bash
echo $PATH
```

Example:

```bash
/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
```

---

# Understanding PATH

When we run commands like:

```bash
ls
```

Linux searches inside these directories to find the executable command.

If the command location is not present inside PATH, Linux shows:

```bash
command not found
```