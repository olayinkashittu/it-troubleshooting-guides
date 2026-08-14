# Linux SSH Troubleshooting

## Overview

SSH (Secure Shell) is commonly used to remotely administer Linux systems.

## Common SSH Problems

- SSH connection refused
- Connection timed out
- Permission denied
- Incorrect username
- SSH service is not running
- Firewall blocking SSH
- Incorrect IP address or hostname

## 1. Check Network Connectivity

Test the server:

```bash
ping <server-ip>
```

Example:

```bash
ping 192.168.1.10
```

## 2. Test SSH Connection

 Use:
 
```bash
ssh username@server-ip
```

Example:

```bash
ssh admin@192.168.1.10
```

## 3. Check the SSH Service

On the Linux server, check the SSH service:
 
```bash
sudo systemctl status ssh
```

On some distributions the service may be named:

```bash
sudo systemctl status sshd
```

## 4. Start the SSH Service

If the service is stopped:
 
```bash
sudo systemctl start ssh
```

Or:

```bash
sudo systemctl start sshd
```

## 5. Enable SSH at Startup

Use:
 
```bash
sudo systemctl enable ssh
```

Or:

```bash
sudo systemctl enable sshd
```

## 6. Check Listening Ports

Use:
 
```bash
ss -tuln
```

SSH normally listens on TCP port:

```bash
22
```
