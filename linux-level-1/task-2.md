# Linux Task 2: User and Group Management

## Step 1: Check App Server Details and Login

```bash
ssh <username>@<ip address>
```

## Step 2: Check if User Exists

```bash
id <user>
```

## Step 3A: If User Exists - Create Group and Add User

If the user exists, create the group and add the user to it:

```bash
sudo groupadd <group_name>

sudo usermod -aG <group_name> <username>
```

## Step 3B: If User Doesn't Exist - Create User

If the user doesn't exist, create the user:

```bash
sudo useradd <username>
```

## Step 4: Repeat for All App Servers

Perform the same steps on all app servers.



