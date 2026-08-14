# Linux User Management Troubleshooting

## Overview

Linux user management involves creating, modifying, disabling, and removing user accounts and managing their group membership.

## Common User Management Issues

- User cannot log in.
- User account does not exist.
- User has incorrect permissions.
- User is not a member of the required group.
- User account is locked or expired.
- User cannot access a required resource.

## 1. Check the Current User

Use:

```bash
whoami
```

This displays the username of the currently logged-in user.

## 2. View User Information

Use:

```bash
id username
```

This displays the user's UID, primary group, and supplementary groups.

## 3. List Users

To view local user accounts:

```bash
cat /etc/passwd
```

## 4. Create a User

Use:

```bash
sudo useradd username
```

On many Linux distributions, you can also use:

```bash
sudo adduser username
```

Follow the prompts when required.

## 5. Set or Change a Password

Use:

```bash
sudo passwd username
```

Enter the new password when prompted.

## 6. Add a User to a Group

Use:

```bash
sudo usermod -aG groupname username
```

Example:

```bash
sudo usermod -aG sudo username
```

Use the appropriate administrative group for the Linux distribution and organizational policy.

## 7. Check Group Membership

Use:

```bash
groups username
```

or:

```bash
id username
```

## 8. Lock a User Account

To temporarily prevent interactive login:

```bash
sudo passwd -l username
```

## 9. Unlock a User Account

To unlock the account:

```bash
sudo passwd -u username
```

## 10. Delete a User

Use caution when removing accounts.

```bash
sudo userdel username
```

To remove the user's home directory where appropriate:

```bash
sudo userdel -r username
```

Only use this when the organization's retention and data policies permit it.

## Troubleshooting Login Problems

If a user cannot log in:

1. Confirm the username is correct.
2. Check whether the account exists.
3. Check whether the account is locked.
4. Check password status.
5. Check account expiration.
6. Check group membership.
7. Review relevant system logs.
8. Verify file and home-directory permissions.

## Useful Commands

```bash
whoami
```

```bash
id username
```

```bash
groups username
```

```bash
passwd -S username
```

```bash
getent passwd username
```

## Verification

After making changes:

```bash
id username
```

Confirm that the account has the expected UID and group membership.

Test the user's ability to log in and access the required resources.

## Security Best Practice

Use the principle of least privilege. Grant users only the permissions and group memberships required for their responsibilities.

Never record passwords in troubleshooting documentation.

## Resolution

The Linux user account was reviewed and the required account, password, group, or access settings were corrected.

