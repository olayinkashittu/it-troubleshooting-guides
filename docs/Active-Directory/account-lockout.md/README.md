# Active Directory Account Lockout Troubleshooting

## Issue

A user is unable to sign in because their Active Directory account has been locked.

## Common Causes

- Multiple incorrect password attempts
- An old password saved on a device
- A mapped network drive using an old password
- A mobile device or email application using old credentials
- A scheduled task or service using outdated credentials

## Troubleshooting Steps

### 1. Verify the user's identity

Confirm the user's identity according to the organization's security procedures.

### 2. Locate the user account

Open:

```text
Server Manager
→ Tools
→ Active Directory Users and Computers
```

Navigate to the appropriate Organizational Unit (OU) and locate the user account.

### 3. Check whether the account is locked

Right-click the user account and select:

```text
Properties
```

Review the account settings and determine whether the account is locked.

### 4. Unlock the account

Right-click the user account and select:

```text
Reset Password
```

or use the account options available in your Active Directory environment to unlock the account.

### 5. Reset the password when necessary

If the user has forgotten the password or the password is suspected to be compromised, reset it according to organizational policy.

### 6. Identify the cause

Check whether the user has:

- An old password saved on another computer
- A mobile device using the old password
- Stored Windows credentials
- A mapped network drive
- A scheduled task using outdated credentials

### 7. Test the account

Ask the user to sign in again and confirm access to required resources.

## Resolution

The user's account was unlocked and successful authentication was confirmed.

## Security Note

Always verify the user's identity before unlocking or resetting an account.

