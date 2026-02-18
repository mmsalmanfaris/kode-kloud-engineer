# Linux Task 7: Disable Root SSH Login

## Step 1: Login to App Server

```bash
ssh <user>@<ip>
```

## Step 2: Edit SSH Configuration File

```bash
sudo vi /etc/ssh/sshd_config
```

## Step 3: Find and Modify PermitRootLogin

Find the line containing `PermitRootLogin` and change the value from `yes` to `no`.

## Step 4: Save the File

Press `Esc` and then type `:wq!` to save and exit the editor.

## Step 5: Restart SSH Service

```bash
sudo systemctl restart sshd
```

## Step 6: Exit the Server

```bash
exit
```

## Step 7: Verify Root Login is Disabled

Attempt to login as root:

```bash
ssh root@<ip>
```

You should receive a **permission denied** error, confirming root login is disabled.
