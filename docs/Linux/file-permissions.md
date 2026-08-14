# Linux File Permissions Troubleshooting

## Overview

Linux file permissions control who can read, write, or execute files and directories.

Permissions are commonly assigned to:

- Owner
- Group
- Other users

## Common Permission Problems

- Permission denied
- User cannot modify a file
- User cannot access a directory
- Script cannot be executed
- Incorrect ownership

## 1. Check File Permissions

Use:

```bash
ls -l
```

Example:
 
```bash
-rwxr-xr--
```

The permission string represents:
 
```bash
Owner | Group | Others
```

## 2. Check File Ownership

Use:

```bash
ls -l filename
```

## 3. Change File Permissions

Use:

```bash
chmod 644 test.txt
```
This gives:

Owner: read and write
Group: read
Others: read

## 4. Make a Script Executable

Use:

```bash
chmod +x script.sh
```

Then run:

```bash
./script.sh
```

## 5.Change File Ownership

Use:

```bash
sudo chown username filename
```

To change both owner and group:

```bash
sudo chown username:groupname filename
```
## 6. Check Directory Permissions

Use:

```bash
ls -ld directory
```
A user may have access to a file but still be unable to enter its directory if the directory permissions are incorrect.

## 7. Troubleshoot "Permission Denied"

When a user receives a permission error:

Check the file permissions.
Check the file owner.
Check the group membership.
Check directory permissions.
Verify whether sudo is required.
Apply the minimum permissions necessary.

## Useful Commands

```bash
ls -l
```

```bash
chmod
```

```bash
chown
```

```bash
id
```

```bash
groups
```

Verification

After changing permissions:

```bash
ls -l filename
```

Then test the required action again.

Best Practice

Follow the principle of least privilege. Do not give users full access when only limited permissions are required.

Avoid using:

```bash
chmod 777
```
unless there is a specific, controlled reason in a lab environment.

