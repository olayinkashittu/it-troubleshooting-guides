# DNS Troubleshooting

## Common Symptoms

- Websites do not open.
- Hostnames cannot be resolved.
- Network access is unavailable.

## Troubleshooting Steps

### Check the DNS configuration

```cmd
ipconfig /all
```

### Test DNS resolution

```cmd
nslookup google.com
```

### Flush the DNS cache

```cmd
ipconfig /flushdns
```

## Resolution

DNS service restored.

git add .

git commit -m "Added networking troubleshooting documentation"

git push origin main
