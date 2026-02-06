# DevOps Day 09: MariaDB Permissions Fix

## Step 1: Check Database Credentials

Check the database credentials.

## Step 2: Login to the Server

Login to the server using SSH.

## Step 3: Check MariaDB Status

```bash
systemctl status mariadb
```

## Step 4: Check Permissions

```bash
ls -ld /var/lib/mysql
```

## Step 5: Fix Ownership and Permissions

Run these commands in the terminal to provide access to MariaDB:

```bash
chown -R mysql:mysql /var/lib/mysql
chmod 755 /var/lib/mysql
```

## Step 6: Recheck MariaDB Status

```bash
systemctl status mariadb
```