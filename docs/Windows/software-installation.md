# Software Installation Troubleshooting Guide

## Overview

Software installation failures are common in IT support environments. Problems may occur because of insufficient permissions, corrupted installation files, incompatible operating systems, missing dependencies, or antivirus restrictions.

This guide provides a step-by-step troubleshooting process for diagnosing and resolving software installation issues on Windows systems.

---

## Common Symptoms

```bash
- Installation freezes or stops unexpectedly
- Error messages appear during installation
- Setup files fail to launch
- "Access Denied" errors
- Installation completes, but the application does not open
- The application crashes immediately after installation
- Missing DLL or dependency errors
```

## Troubleshooting Steps

### 1. Verify System Requirements

Before installing any software, confirm that the computer meets the minimum requirements.

Check:

```bash
- Operating system version
- Processor requirements
- RAM requirements
- Available disk space
- Required software dependencies
```

### 2. Run the Installer as Administrator

Some applications require administrative privileges.

**Steps:**

```bash
1. Locate the installation file.
2. Right-click the installer.
3. Select **Run as administrator**.
4. Follow the installation wizard.
```

### 3. Check Available Disk Space

Open:

```bash
Settings → System → Storage
```

Alternatively, use PowerShell:

```bash 
Get-PSDrive -PSProvider FileSystem
```
