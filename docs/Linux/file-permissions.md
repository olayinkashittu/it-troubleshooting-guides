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
