# Azure Task 37: Configure MySQL and PHP VMs

## Step 1: Login to Azure Portal

Login to the Azure portal.

## Step 2: Create MySQL VM

Create the VM using the specific information provided:
- Image
- Location
- Security type
- Standard SSD

## Step 3: Set Up Inbound Rule

Set up inbound rule for the VM on port **3306**.

## Step 4: SSH into MySQL VM

SSH into the MySQL VM.

## Step 5: Switch to MySQL Mode

Connect to MySQL.

## Step 6: Create Database

```sql
CREATE DATABASE datacenter_db;
```

## Step 7: Create User

```sql
CREATE USER 'datacenter_user'@'%' IDENTIFIED BY 'password123';
```

## Step 8: Grant Privileges

```sql
GRANT ALL PRIVILEGES ON datacenter_db.* TO 'datacenter_user'@'%';
FLUSH PRIVILEGES;
```

## Step 9: SSH into PHP VM

SSH into the PHP VM.

## Step 10: Edit Configuration File

```bash
sudo vi /var/www/html/db_test.php
```

Update the MySQL VM IP and database details that were created.

## Step 11: Test the Connection

Access the following URL in your browser:

```
http://<php-vm-public-ip>/db_test.php
```

## Expected Response

You should see:

```
Connected successfully
```
