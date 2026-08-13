# Network Connectivity Troubleshooting

## Issue

The computer cannot access the network or the internet.

## Troubleshooting Steps

### 1. Check the physical connection

- Verify that the Ethernet cable is connected.
- Verify that Wi-Fi is enabled.
- Check for network adapter errors.

### 2. Verify the IP configuration

```cmd
ipconfig
```

### 3. Release and renew the IP address

```cmd
ipconfig /release
ipconfig /renew
```

### 4. Test network connectivity

```cmd
ping 8.8.8.8
```

### 5. Check DNS resolution

```cmd
nslookup google.com
```

### 6. Restart the network adapter

- Disable the adapter.
- Enable the adapter.
- Test the connection again.

## Resolution

Network connectivity restored successfully.
