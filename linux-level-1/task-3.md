# Linux Task 3: Create User Without Shell

## Step 1: Login to the Server

Login to the server.

## Step 2: Switch to Root User

```bash
sudo -i
```

## Step 3: Create User Without Shell

```bash
useradd -s /sbin/nologin <username>
```