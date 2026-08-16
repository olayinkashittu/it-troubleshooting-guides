# Active Directory Organizational Units (OUs)

## Overview

An Organizational Unit (OU) is a container in Active Directory used to organize users, computers, groups, and other objects.

OUs help administrators apply Group Policy and manage resources according to departments, locations, or business functions.

## Example OU Structure

```bash
company.local
│
├── IT
├── HR
├── Finance
├── Sales
├── Management
└── Computers
```

## Create an Organizational Unit

### 1. Open Active Directory Users and Computers

On the domain controller:

Server Manager
```bash
→ Tools
→ Active Directory Users and Computers
```

### 2. Select the domain

Expand your domain in the left-hand navigation pane.

For example:

```bash
company.local
```

### 3. Create the OU

Right-click the domain and select:

New
```bash
→ Organizational Unit
```

Enter the OU name.

Example:

```bash
IT
```

Click **OK**.

## Create Departmental OUs

You can create separate OUs for different departments.

Example:

```bash
company.local
│
├── IT
├── HR
├── Finance
├── Sales
└── Management
```

This makes it easier to manage users and computers.

## Move a User into an OU

To move a user:

1. Locate the user account.
2. Right-click the account.
3. Select **Move**.
4. Choose the destination OU.
5. Click **OK**.

Example:

```bash
Users
   ↓
IT OU
```

## Move a Computer into an OU

Computers can also be organized into OUs.

For example:

```bash
Computers
   ↓
IT-Computers
```

This can help administrators apply computer-specific Group Policies.

## OU and Group Policy

One of the main purposes of OUs is to organize objects so that Group Policy can be applied appropriately.

Example:

```bash
IT OU
   ↓
IT Security GPO
   ↓
Users and computers in the OU
```

## Troubleshooting OU Issues

### User is receiving the wrong Group Policy

Check:

- The user's current OU.
- GPO links.
- Group Policy inheritance.
- Security filtering.

### Computer is receiving unexpected settings

Check:

- The computer's OU.
- Linked GPOs.
- Group Policy inheritance.
- `gpresult /r`.

Use:

```bash
gpresult /r
```

for a summary of applied policies.

## Best Practices

- Use clear and consistent OU names.
- Organize users and computers logically.
- Avoid creating unnecessary OUs.
- Document important OU changes.
- Test Group Policy changes before applying them broadly.
- Restrict administrative permissions according to the principle of least privilege.

## Example Lab Structure

For an IT Support practice lab, you could create:

```bash
LAB.local
│
├── IT
│   └── IT-Computers
│
├── HR
│   └── HR-Computers
│
├── Finance
│   └── Finance-Computers
│
└── Sales
    └── Sales-Computers
```

## Verification

After creating an OU:

- Confirm the OU appears in Active Directory Users and Computers.
- Verify that users or computers are in the correct OU.
- Confirm required Group Policies apply correctly.

## Resolution

The Active Directory Organizational Unit structure was created and organized to support effective user, computer, and Group Policymanagement.

