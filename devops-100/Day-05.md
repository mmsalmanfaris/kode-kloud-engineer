## Day 04

To connect to a remote server:

```bash
ssh user@hostname
```

Check the OS

```bash
cat /etc/os-release
```

Install SELinux

```bash
sudo yum install -y selinux-policy selinux-policy-targeted
```

Disable the SELinux

```bash
vi /etc/selinux/config
```

Update SELINUX= to 

```bash
SELINUX=disabled
```


Check the file status
```bash
grep SELINUX= /etc/selinux/config
```
