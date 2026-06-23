# Users and Permissions

![Users and Permissions Commands](./images/users-and-permissions-commands.jpg)

## Objective

Learn how Linux manages users, groups and file permissions.

Understanding permissions is essential for cybersecurity because incorrect permissions can expose sensitive data or allow attackers to gain elevated privileges.

---

## Linux User Types

Linux contains several user types.

### Root User

- UID 0
- Full administrative privileges
- Can access every file
- Can modify system configuration

Example:

```bash
sudo su
```

---

### Standard User

Normal user account used for everyday work.

Benefits include:

- Reduced security risk
- Less chance of accidental system damage
- Better auditing

Display current user:

```bash
whoami
```

---

### System Users

System accounts run services such as:

- www-data
- mysql
- nobody

View all users:

```bash
cat /etc/passwd
```

---

## Groups

Groups allow multiple users to share permissions.

Display groups:

```bash
groups
```

Display current user ID:

```bash
id
```

---

## File Permissions

Linux permissions are divided into three categories.

Owner

Group

Others

Each has:

Read (r)

Write (w)

Execute (x)

Example:

```bash
ls -l
```

Example output:

```
-rwxr-xr--
```

Meaning:

Owner:
Read
Write
Execute

Group:
Read
Execute

Others:
Read only

---

## Changing Permissions

Add execute permission

```bash
chmod +x filename
```

Numeric permissions

```bash
chmod 755 filename
```

Permission values

Read = 4

Write = 2

Execute = 1

Examples

755

Owner = 7 (rwx)

Group = 5 (r-x)

Others = 5 (r-x)

644

Owner = rw-

Group = r--

Others = r--

---

## Changing Ownership

```bash
sudo chown username filename
```

Change group

```bash
sudo chgrp groupname filename
```

---

## Cybersecurity Relevance

Permissions protect systems from:

Unauthorised access

Privilege abuse

Malware

Accidental modification

Every security professional must understand Linux permissions because most enterprise servers run Linux.

---

## Practical Exercises

Run:

```bash
whoami
```

Run:

```bash
id
```

Run:

```bash
groups
```

Run:

```bash
ls -l
```

Run:

```bash
cat /etc/passwd

## Skills Demonstrated

✔ Linux user management

✔ User identification

✔ Group management

✔ Linux permissions

✔ Cybersecurity fundamentals

---

## Reflection

Learning Linux permissions has shown me how operating systems protect files and users through privilege separation.

This knowledge is fundamental for cybersecurity roles including SOC Analyst, Security Engineer and Penetration Tester.
