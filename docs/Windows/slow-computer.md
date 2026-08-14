# Windows Slow Computer Troubleshooting

## Issue

A Windows computer is running slowly, taking a long time to start, or applications are responding slowly.

## Common Symptoms

- Slow startup
- Applications take a long time to open
- High CPU usage
- High memory usage
- High disk usage
- System freezes
- Slow file operations
- Browser performance problems

## Troubleshooting Steps

### 1. Check Task Manager

Press:

```bash
Ctrl + Shift + Esc
```

### Open Task Manager.

Review:

CPU usage
Memory usage
Disk usage
Network usage

Identify applications or processes consuming unusually high resources.

### 2. Check Startup Applications

In Task Manager:

```bash
Startup apps
```

Review programs that start automatically with Windows.

Disable unnecessary startup applications when authorized.

### 3. Check Available Disk Space

Open:

```bash
Settings
→ System
→ Storage
```

Check available free space.

Remove unnecessary files using approved Windows cleanup tools.

### 4. Delete Temporary Files

Open:

```bash
Settings
→ System
→ Storage
→ Temporary files
```

Review the listed temporary files and remove unnecessary items.

### 5. Check for Malware

Run an approved antivirus or Microsoft Defender scan.

Do not disable security software simply to improve performance.

### 6. Check Windows Updates

Go to:

```bash
Settings
→ Windows Update
```

Install available updates according to organizational policy.

### 7. Check System Resource Usage

From Task Manager, identify whether the problem is primarily related to:

CPU
Memory
Disk
Network

This helps narrow down the cause.

### 8. Check Running Applications

Close applications that are not required.

Check whether a particular application consistently causes high resource usage.

### 9. Restart the Computer

Restart Windows and check whether performance improves.

### 10. Check Hardware

If software troubleshooting does not resolve the issue, investigate:

Available RAM
Storage type
Storage health
CPU performance
Overheating
Hardware errors

## Useful Commands

### Check System Information

```bash
   cmd
systeminfo
```
Check Running Processes

```bash
cmd
tasklist
```
