# Microsoft Outlook Troubleshooting

## Issue

Microsoft Outlook is not sending or receiving emails, is slow, or is displaying connection errors.

## Common Symptoms

- Outlook is offline.
- Emails are not sending.
- Emails are not being received.
- Outlook is slow or freezing.
- Mailbox synchronization is failing.
- Outlook repeatedly asks for a password.

## Troubleshooting Steps

### 1. Check the internet connection

Confirm that the computer has a working network or internet connection.

Test connectivity with:

```cmd
ping 8.8.8.8
```

### 2. Check Outlook connection status

Open Outlook and check the status shown at the bottom of the window.

Look for messages such as:

```text
Connected
Working Offline
Disconnected
```

If Outlook is offline, select:

```text
Send / Receive
→ Work Offline
```

and make sure Work Offline is disabled.

### 3. Check mailbox storage

Verify that the mailbox has available storage.

A full mailbox may prevent new messages from being received.

### 4. Check the Outlook account

Go to:

```text
File
→ Account Settings
→ Account Settings
```

Verify that the correct account is configured.

### 5. Test Outlook on the web

Sign in to the organization's Microsoft 365 webmail service using the user's authorized account.

If webmail works but the desktop application does not, the issue may be related to the Outlook client or local profile.

### 6. Restart Outlook

Close Outlook completely and open it again.

If necessary, restart the computer.

### 7. Create a new Outlook profile

Open:

```text
Control Panel
→ Mail
→ Show Profiles
```

Create a new profile and configure the user's account according to organizational procedures.

### 8. Test sending and receiving

Send a test email to an authorized test account and confirm that:

- The message leaves the Outbox.
- The recipient receives the message.
- A reply is received successfully.

## Verification

Confirm that Outlook:

- Connects successfully.
- Sends emails.
- Receives emails.
- Synchronizes the mailbox correctly.

## Resolution

The Outlook issue was identified and resolved after checking connectivity, account configuration, mailbox status, and the Outlook client.

## Security Best Practice

Never request or record a user's password in troubleshooting documentation. Use approved authentication and account-recovery procedures.

