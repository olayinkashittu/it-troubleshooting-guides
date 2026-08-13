# Linux Networking Commands Troubleshooting

## Overview

Linux provides several command-line tools for checking network configuration, testing connectivity, troubleshooting DNS, and identifying network-related problems.

## 1. Check Network Interfaces

Use:

```bash
ip addr
```

## 2. Check the Routing Table

 Use:
 
```bash
ip route
```

## 3. Test Network Connectivity

 Use:
 
```bash
ping 8.8.8.8
```

## 4. Test DNS Resolution

 Use:
 
```bash
ping google.com
```

Use:

```bash
nslookup google.com
```

Use:

```bash
dig google.com
```

## 5. Check Open Network Connections

 Use:
 
```bash
ss -tuln
```
