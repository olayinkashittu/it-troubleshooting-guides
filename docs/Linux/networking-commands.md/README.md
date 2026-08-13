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

Use:
 
```bash
ss -tunap
```

## 6. Check the Hostname

 Use:
 
```bash
hostname
```

Use:
 
```bash
hostnamectl
```

## 7. Trace the Network Path

 Use:
 
```bash
traceroute google.com
```

An alternative is:
 
```bash
tracepath google.com
```

## 8. Check DNS Configuration

 Use:
 
```bash
cat /etc/resolv.conf
```

## 9. Troubleshooting Sequence

 When a Linux system cannot access the network, check in this order:
 
```bash
Network interface
      ↓
IP address
      ↓
Default gateway
      ↓
External IP connectivity
      ↓
DNS resolution
      ↓
Application/service connectivity
```

Useful Tests 
Check the interface:
 
```bash
ip addr
```

Check the route:
 
```bash
ip route
```

Test the gateway:
 
```bash
ping <gateway-ip>
```

Test an external IP:
 
```bash
ping 8.8.8.8
```

Test DNS:
 
```bash
ping google.com
```

```bash
## Common Symptoms and Causes

### No IP address

Possible causes:

- DHCP failure
- Disabled network interface
- Incorrect static configuration

### Can ping IP but not hostname

Possible cause:

- DNS configuration problem

### Cannot ping the gateway

Possible causes:

- Incorrect IP configuration
- Incorrect subnet
- Network interface problem
- Local network connectivity problem

### Can reach the gateway but not the internet

Possible causes:

- Default gateway issue
- Router problem
- Firewall rules
- Upstream connectivity issue

## Verification

Confirm:

- The network interface is active.
- A valid IP address is assigned.
- A default route exists.
- The gateway responds.
- External IP addresses can be reached.
- DNS names resolve correctly.

## Useful Command Summary

```bash
ip addr
```

```bash
ping 8.8.8.8
```

```bash
nslookup google.com
```

```bash
ss -tuln
```

```bash
hostname
```

```bash
traceroute google.com
```
