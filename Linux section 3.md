# User Management in Linux

## Understanding User Management

For example:

When you purchase a new laptop, you first create:

- Admin User
- Password

Then you may create non-admin users for other people.

Similarly, Linux uses User Management to:

- Secure the Linux server
- Control user access
- Avoid system malfunction
- Manage permissions using users and groups

---

# Creating Users in Linux

## Create User

```bash
useradd abhi
```

Creates a new user named `abhi`.

---

## Check User is Created or Not

```bash
cat /etc/passwd
```

OR

```bash
vim /etc/passwd
```

This file stores all Linux user information.

---

# Set Password for User

```bash
passwd abhi
```

Creates or updates the password for user `abhi`.

---

# Check Encrypted Passwords

```bash
cat /etc/shadow
```

The `/etc/shadow` file stores encrypted passwords.

Passwords are encrypted for security reasons.

---

# Delete User

```bash
userdel abhi
```

Deletes the user.

---

# Verify User Deletion

```bash
cat /etc/passwd
```

Checks whether the user still exists.

---

# Create User with Home Directory

```bash
adduser abhi
```

This command:
- Creates the user
- Creates home directory
- Asks for additional details

---

# Check Home Directory

```bash
ls /home/
```

Displays all user home directories.

---

# Switch User

```bash
su - abhi
```

Switches to user `abhi`.

---

# Check Current User

```bash
whoami
```

Displays the currently logged-in user.

---

# Password Policies in Linux

## Password Expiry

If the organization requires password change every 90 days:

```bash
chage -M 90 username
```

Example:

```bash
chage -M 90 abhi
```

Sets password expiry to 90 days.

---

# Lock User Account

```bash
passwd -l username
```

Example:

```bash
passwd -l abhi
```

Locks the user account.

---

# Unlock User Account

```bash
passwd -u username
```

Example:

```bash
passwd -u abhi
```

Unlocks the user account.

---

# Interview Questions

## Difference Between `useradd` and `adduser`

### `useradd`

- Quick way to create user
- Basic command
- Does not ask for user details

---

### `adduser`

- More powerful command
- Creates home directory automatically
- Prompts for user details

---

# Can Password Be Restored?

## Answer

No.

Passwords are stored in encrypted format inside:

```bash
/etc/shadow
```

They cannot be viewed in original form.

---

# Group Management in Linux

## Why Do We Need Groups?

Example:

Suppose an organization has:
- 100 users
- Multiple teams
- Different permissions

Teams may include:
- Dev
- QA
- DevOps
- Management

Instead of changing permissions user-by-user, we manage permissions using groups.

---

# Create Group

```bash
groupadd devsecops
```

Creates a new group named `devsecops`.

---

# Add User to Group

```bash
usermod -aG devsecops abhi
```

OR

```bash
usermod -aG groupname username
```

Example:

```bash
usermod -aG devsecops abhi
```

Adds user `abhi` to the `devsecops` group.

---

# SSH in Linux

When you join a company, the admin usually provides:

- Server IP Address
- Username
- Password

To connect to the server remotely, Linux uses SSH.

---

# What is SSH?

SSH stands for:

```text
Secure Shell
```

Used for secure remote login.

---

# SSH Components

## SSH Client

Used to connect to remote servers.

Popular SSH clients:
- Git Bash
- OpenSSH
- PuTTY

---

## SSHD Service

Linux server runs a service called:

```text
sshd
```

This service allows remote login to the server.

---

# SSH Configuration File

Sometimes cloud providers disable password authentication.

Check configuration file:

```bash
/etc/ssh/sshd_config
```

OR

```bash
/etc/ssh/sshd_config.d/60-cloudimg-settings.conf
```

---

# Restart SSH Service

After changing SSH configuration:

```bash
systemctl restart ssh
```

Restarts the SSH service.