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

```text
Device Manager
