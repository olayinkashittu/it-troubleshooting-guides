# Windows Blue Screen Troubleshooting

## Issue

A Windows computer displays a blue screen error, suddenly restarts, or crashes with a stop code.

## Common Symptoms

- Blue Screen of Death (BSOD)
- Unexpected restart
- System crash
- Stop code displayed
- Windows fails to start normally
- Repeated crashes

## Troubleshooting Steps

### 1. Record the Stop Code

When the blue screen appears, record the displayed stop code.

Examples include:

- `CRITICAL_PROCESS_DIED`
- `MEMORY_MANAGEMENT`
- `PAGE_FAULT_IN_NONPAGED_AREA`
- `SYSTEM_SERVICE_EXCEPTION`

The stop code can help identify the likely cause.

### 2. Restart the Computer

Restart Windows and check whether the problem happens again.

If the issue is recurring, continue troubleshooting.

### 3. Check Recently Installed Software or Drivers

Consider whether the problem began after:

- Installing a new driver
- Installing new software
- Installing a Windows update
- Connecting new hardware

Remove or roll back the suspected change when appropriate and authorized.

### 4. Start Windows in Safe Mode

If Windows cannot start normally, use the Windows Recovery Environment to access **Safe Mode**.

Safe Mode loads Windows with a limited set of drivers and services.

### 5. Check Device Manager

Open:

```bash
Device Manager
```

Look for devices showing warning symbols.

Review recently updated or newly installed drivers.

### 6. Update or Roll Back Drivers

If a driver is suspected:

Install an approved updated driver.
Roll back the driver if the problem began after an update.
Restart the computer and test again.

### 7. Run System File Checker

Open Command Prompt as Administrator and run:

```bash
sfc /scannow
```
Wait for the scan to complete.

### 8. Run DISM

If Windows component corruption is suspected, run:

```bash
DISM /Online /Cleanup-Image /RestoreHealth
```

Allow the process to complete before restarting the computer.

### 9. Check Windows Memory

Use the Windows Memory Diagnostic tool when memory problems are suspected.

Open

Windows Memory Diagnostic
```bash
Follow the prompts to restart and test the computer's memory.
```

### 10. Check Disk Health

Open Command Prompt as Administrator and run:

```bash
chkdsk
```
Additional repair options should only be used when appropriate and according to support procedures.

### 11. Review Windows Update History

Open:

Settings
```bash
→ Windows Update
→ Update history
```
Look for updates installed shortly before the crashes started.

### 12. Check Event Viewer

Open:

```bash
Event Viewer
```

Review relevant system and application errors around the time of the crash.

Common Causes
Faulty or incompatible drivers
Corrupted system files
Faulty RAM
Storage problems
Hardware failures
Problematic software
Windows update issues
Overheating
Malware

### Useful Commands

Check system files:

```bash
sfc /scannow
```
Repair Windows components:

```bash
DISM /Online /Cleanup-Image /RestoreHealth
```

Check the disk:
```bash
chkdsk
```

Display system information:

```bash
systeminfo
```

### Verification

Confirm that:

Windows starts normally.
The blue screen does not reoccur.
The suspected driver or software issue has been resolved.
Hardware diagnostics do not report errors.
Windows system files are healthy.
The user can operate the computer normally.

### Security Best Practice

Only install drivers and software from trusted and authorized sources. Do not disable security controls simply to bypass a crash.

### Resolution

The blue screen issue was isolated by reviewing the stop code, recent changes, drivers, system files, memory, storage, updates, and hardware.
