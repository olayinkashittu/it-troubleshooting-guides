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

## 7. Check the Firewall

For systems using UFW:
 
```bash
For systems using UFW
```

If SSH is authorized and the firewall is blocking it:

```bash
sudo ufw allow ssh
```

Only make firewall changes that are permitted by the system administrator or lab configuration.

## 8. Check the SSH Configuration

The main SSH server configuration file is:
 
```bash
/etc/ssh/sshd_config
```

Check the configuration carefully before making changes.

## 9. Permission Denied

If you receive:
 
```bash
If you receive
```

Check:

Username
Password or SSH key
Account status
SSH access permissions
Home-directory permissions
SSH server configuration

## 10. Connection Refused

If you receive:
 
```bash
If you receive
```

Possible causes include:

SSH service is stopped.
SSH is listening on another port.
Firewall is blocking the connection.
SSH server is not installed.

## 11. Connection Timed Out

Possible causes:

Incorrect IP address
Network connectivity problem
Firewall blocking traffic
Server is offline
Routing problem

## Useful Commands
 
```bash
ping <server-ip>
```

```bash
ssh username@server-ip
```

```bash
sudo systemctl status ssh
```

```bash
ss -tuln
```

```bash
sudo ufw status
```
## Verification

Confirm:

The Linux server is reachable.
SSH is running.
The correct port is listening.
Firewall rules permit authorized SSH access.
The user can authenticate successfully.
Security Best Practice

Use strong authentication, restrict SSH access to authorized users, and avoid exposing SSH unnecessarily to untrusted networks.

Never document or share real passwords or private SSH keys.

## Resolution

The SSH connectivity issue was isolated by checking network connectivity, the SSH service, listening ports, firewall configuration, and authentication.
