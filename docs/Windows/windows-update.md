# Windows Update Troubleshooting

## Issue

Windows Update fails, repeatedly reports an error, or does not install available updates.

## Common Symptoms

- Windows Update fails.
- Updates remain stuck at a percentage.
- An error code is displayed.
- Windows repeatedly attempts to install the same update.
- Updates are not detected.
- The computer restarts unexpectedly during an update.

## Troubleshooting Steps

### 1. Check the Internet Connection

Confirm that the computer has a stable network connection.

Test connectivity with:

```cmd
ping 8.8.8.8
```

### 2. Restart the Computer

Restart Windows and check for updates again.

Open:

```text
Settings
→ Windows Update
```

Then select:

```text
Check for updates
```

### 3. Run the Windows Update Troubleshooter

Open:

```text
Settings
→ System
→ Troubleshoot
→ Other troubleshooters
```

Locate:

```text
Windows Update
```

Select:

```text
Run
```

Follow the recommendations provided by Windows.

### 4. Check Available Storage

Open:

```text
Settings
→ System
→ Storage
```

Confirm that sufficient free disk space is available.

Insufficient storage can prevent updates from installing successfully.

### 5. Check Windows Update Services

Open:

```text
Services
```

Check the status of services such as:

```text
Windows Update
Background Intelligent Transfer Service (BITS)
Cryptographic Services
```

Follow organizational procedures before changing service settings.

### 6. Clear the Windows Update Cache

If Windows Update repeatedly fails, the update cache may need to be rebuilt.

An administrator can stop the relevant services, clear the update cache directories, and restart the services according to the organization's approved support procedure.

### 7. Run System File Checker

Open Command Prompt as Administrator and run:

```cmd
sfc /scannow
```

Wait for the scan to complete.

### 8. Run DISM

If system component corruption is suspected, run:

```cmd
DISM /Online /Cleanup-Image /RestoreHealth
```

Allow the operation to complete before testing Windows Update again.

### 9. Check the Update History

Open:

```text
Settings
→ Windows Update
→ Update history
```

Review failed updates and note any displayed error codes.

### 10. Restart and Test Again

Restart the computer after troubleshooting.

Return to:

```text
Settings
→ Windows Update
```

Select:

```text
Check for updates
```

## Common Causes

- Unstable internet connection
- Insufficient disk space
- Corrupted Windows Update cache
- Damaged system files
- Windows Update service problems
- Pending restart
- Update compatibility problems
- Organizational update policies

## Useful Commands

Check system files:

```cmd
sfc /scannow
```

Repair the Windows component store:

```cmd
DISM /Online /Cleanup-Image /RestoreHealth
```

Test network connectivity:

```cmd
ping 8.8.8.8
```

## Verification

Confirm that:

- Windows Update can connect successfully.
- Available updates are detected.
- Updates download successfully.
- Updates install successfully.
- No recurring error is displayed.
- The computer restarts normally.

## Security Best Practice

Install Windows updates through approved Microsoft and organizational update channels. Do not bypass security controls or disable protection mechanisms simply to force an update.

## Resolution

The Windows Update issue was isolated by checking connectivity, storage, update services, system integrity, update history, and Windows Update configuration.
