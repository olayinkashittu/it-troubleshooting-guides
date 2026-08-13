# Active Directory User Management

## Overview

Active Directory Users and Computers (ADUC) allows administrators to create and manage domain user accounts.

## Common User Management Tasks

- Create a new user account
- Reset a user password
- Disable a user account
- Enable a disabled account
- Unlock a locked account
- Modify user information
- Move users between Organizational Units (OUs)

## Create a New User

### 1. Open Active Directory Users and Computers

On the domain controller:

```text
Server Manager
→ Tools
→ Active Directory Users and Computers
```

### 2. Select the Organizational Unit

Navigate to the appropriate OU where the new user should be created.

### 3. Create the user

Right-click the OU and select:

```text
New
→ User
```

Enter:

- First name
- Last name
- User logon name

Click **Next**.

### 4. Set the password

Enter a temporary password that complies with the organization's password policy.

You may select:

```text
☑ User must change password at next logon
```

Click **Next** and then **Finish**.

## Disable a User Account

To disable an account:

1. Locate the user.
2. Right-click the account.
3. Select **Disable Account**.
4. Confirm the action.

Disabling an account is commonly used when an employee leaves the organization or when access must be temporarily suspended.

## Enable a User Account

To enable a disabled account:

1. Locate the user.
2. Right-click the account.
3. Select **Enable Account**.
4. Confirm the action.

## Unlock a User Account

When an account is locked:

1. Locate the user account.
2. Open the account properties.
3. Use the available account unlock option.
4. Apply the change.

## Modify User Information

Right-click the user and select:

```text
Properties
```

Administrators can update information such as:

- Department
- Job title
- Telephone number
- Office location
- Description
- Group membership

Only change fields permitted by organizational policy.

## Move a User to Another OU

To move a user:

1. Locate the user.
2. Right-click the account.
3. Select **Move**.
4. Select the destination OU.
5. Confirm the move.

The user's OU determines which Group Policies and administrative controls may apply to the account.

## Verification

After making changes:

- Confirm the correct user account was modified.
- Verify the account status.
- Confirm the user can sign in when appropriate.
- Verify access to required resources.

## Security Best Practice

Follow the principle of least privilege and organizational procedures when managing user accounts. Always verify the identity and authorization of the requester before making account changes.
