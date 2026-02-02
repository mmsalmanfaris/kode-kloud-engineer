## Day 07 | Linux SSH Authentication

Generate a new ssh key pair:

```bash
sssh-keygen -t rsa -b 4096
```

copy the thor ssh to the app server

```bash
ssh-copy-id username@server_ip
```

Thats it now the the thor user can access the app servers without password.
