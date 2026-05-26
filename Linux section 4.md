# File Management in Linux

## List Files and Directories

```bash
ls
```

Used to list files and directories.

---

# Change Directory

## Go Inside Directory

```bash
cd directoryname
```

Example:

```bash
cd Downloads
```

`cd` means:

```text
Change Directory
```

---

## Move Back One Directory

```bash
cd ..
```

Moves one step back from current directory.

---

# Check Current Directory

```bash
pwd
```

`pwd` means:

```text
Present Working Directory
```

Displays the current location.

---

# Create New Directory

```bash
mkdir test
```

`mkdir` means:

```text
Make Directory
```

Creates a new folder.

---

# Remove Empty Directory

```bash
rmdir directoryname
```

Deletes empty directory.

Example:

```bash
rmdir test
```

---

# Create File

```bash
touch filename
```

Example:

```bash
touch demo.txt
```

Creates a new empty file.

---

# Delete File

```bash
rm filename
```

Example:

```bash
rm demo.txt
```

Deletes file.

---

# Delete Directory Forcefully

```bash
rm -rf directoryname
```

Example:

```bash
rm -rf test
```

### Understanding Flags

| Flag | Meaning |
|---|---|
| `-r` | Recursive |
| `-f` | Force Delete |

---

# Copy Files

```bash
cp sourcefile destinationfile
```

Example:

```bash
cp demo.txt demo2.txt
```

Creates duplicate copy of the file.

---

# Rename File

```bash
mv oldfilename newfilename
```

Example:

```bash
mv demo.txt newdemo.txt
```

`mv` is also used for moving files.

---

# File Editing in Linux

## Open File in VIM Editor

```bash
vim filename
```

Example:

```bash
vim demo.txt
```

---

# Modes in VIM Editor

## 1. Normal Mode

Default mode when file opens.

Used for:
- Navigation
- Commands
- Copy/Paste

---

## 2. Insert Mode

Used to edit or type inside file.

Press:

```bash
i
```

to enter insert mode.

---

## 3. Command Mode

Used for:
- Save
- Exit
- Search
- Line Navigation

Press:

```bash
Esc
```

to enter command mode.

---

# Save File in VIM

```bash
:wq
```

### Meaning

| Command | Meaning |
|---|---|
| `w` | Write |
| `q` | Quit |

---

# Exit Without Saving

```bash
:q!
```

Exits file without saving changes.

---

# Jump to Specific Line

If file has 2000 lines:

Press:

```bash
Esc
```

Then:

```bash
:100
```

Moves to line number 100.

---

# Print File Content

```bash
cat filename
```

Example:

```bash
cat demo.txt
```

Displays file content.

---

# Read Large Files

## LESS Command

```bash
less filename
```

Used to read large files.

Unlike VIM:
- Cannot edit file
- Only used for viewing

---

# Print Last Lines of File

```bash
tail -20 demo.txt
```

Displays last 20 lines.

---

# Print First Lines of File

```bash
head -20 demo.txt
```

Displays first 20 lines.

---

# Print File in Reverse Order

```bash
tac filename
```

Displays file content in reverse order.

---

# Write Content Without VIM

## Overwrite File Content

```bash
echo 'hello' > demo.txt
```

This:
- Deletes old content
- Adds new content

---

# Append Content to File

```bash
echo 'hello' >> demo.txt
```

This:
- Keeps old content
- Adds new content at end of file