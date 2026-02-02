## Day 06

To connect to all 3 app servers:

```bash
ssh user@hostname
```

Check the OS

```bash
cat /etc/os-release
```

Install Cronie

```bash
sudo yum install -y cronie
```

Start Crond

```bash
systemctl start crond
systemctl status crond
```

Add a cron function to the crontab (*/5 * * * * echo hello > /tmp/cron_text)

```bash
sudo crontab -e
```

After 6 minutes, run this command to check the output
```bash
cat /tmp/cron_text
```
