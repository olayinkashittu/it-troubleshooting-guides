# Active Directory Group Policy Troubleshooting

## Overview

Group Policy allows administrators to centrally manage Windows computers and users in an Active Directory domain.

## Common Group Policy Issues

- Group Policy settings are not applying.
- A user cannot access a required setting.
- Security policies are not updating.
- Login or startup policies are not being applied.

## Troubleshooting Steps

### 1. Confirm the computer is joined to the domain

On the Windows client, verify that the computer is connected to the correct Active Directory domain.

### 2. Check the user's Organizational Unit

In Active Directory Users and Computers, confirm that the user or computer is located in the correct Organizational Unit (OU).

### 3. Open Group Policy Management

On the domain controller:

```text
Server Manager
→ Tools
→ Group Policy Management
```

### 4. Check the Group Policy Object

Locate the appropriate Group Policy Object (GPO) and verify that it is linked to the correct OU.

### 5. Force a Group Policy update

On the Windows client, open Command Prompt as Administrator and run:

```cmd
gpupdate /force
```

Wait for the update to complete.

### 6. Check the applied policies

Run:

```cmd
gpresult /r
```

This displays the Group Policy settings currently applied to the user and computer.

For a detailed report, use:

```cmd
gpresult /h gp-report.html
```

Open the generated HTML report in a web browser.

### 7. Restart the computer

Some Group Policy settings require the computer to be restarted before they take effect.

## Verification

Confirm that the required policy has been applied successfully to the user or computer.

## Resolution

The Group Policy configuration was reviewed, updated, and successfully applied to the affected system.

## Best Practice

Always test new Group Policy changes with a controlled test OU before applying them broadly to production systems.
