# Microsoft 365 Mailbox Troubleshooting

## Issue

A user is unable to send or receive email, has mailbox storage problems, or is experiencing synchronization issues.

## Common Symptoms

- Emails are not being received.
- Emails remain in the Outbox.
- The mailbox is full.
- Outlook shows synchronization errors.
- New messages are delayed.
- The user cannot access the mailbox.

## Troubleshooting Steps

### 1. Check the user's internet connection

Verify that the user's computer is connected to the network.

Test connectivity with:

```cmd
ping 8.8.8.8
```

### 2. Check Outlook

Open Outlook and verify the connection status.

Check whether Outlook shows:

```text
Connected
Working Offline
Disconnected
```

### 3. Test webmail

Sign in to the organization's Microsoft 365 webmail service using the user's authorized account.

If webmail works but Outlook does not, investigate the Outlook client or profile.

### 4. Check mailbox storage

Verify whether the mailbox has reached its storage limit.

If the mailbox is full:

- Remove unnecessary messages.
- Empty Deleted Items when appropriate.
- Archive messages according to organizational policy.
- Review large attachments.

### 5. Check the Outbox

Open Outlook and check whether messages are stuck in:

```text
Outbox
```

Review any error messages and test sending a small message.

### 6. Check synchronization

Confirm that Outlook is synchronizing with the mailbox.

Restart Outlook and perform a manual send/receive when appropriate.

### 7. Check account status

Verify that the user's Microsoft 365 account is active and properly licensed according to organizational policy.

### 8. Check Microsoft 365 service health

If multiple users are experiencing similar problems, check the organization's Microsoft 365 service health information when authorized.

### 9. Test the mailbox

Send a test email and confirm:

- The message leaves the Outbox.
- The recipient receives it.
- A reply is received.
- New messages appear in the Inbox.

## Verification

Confirm that:

- The mailbox is accessible.
- Email can be sent.
- Email can be received.
- Outlook synchronizes correctly.
- The mailbox has sufficient available storage.

## Resolution

The mailbox issue was resolved after checking connectivity, account status, storage, synchronization, and the Outlook client.

## Security Best Practice

Never include passwords, authentication codes, or confidential mailbox information in troubleshooting documentation.
