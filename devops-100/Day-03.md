## Day 03

To connect to a remote server:

```bash
ssh user@hostname
```

To disable root login:

```bash
sudo vi /etc/ssh/sshd_config
```

Change PermitRootLogin yes to:

```bash
PermitRootLogin no
```

Restart the sshd:

```bash
systemctl restart sshd
```

### Repeat on All 3 App Servers
### If 'PermitRootLogin' is commented out, uncomment it and set its value to 'no' for improved security: