# Linux Task 1

## Step 1: Login to the App Server

```bash
ssh <username>@<ip address>
```

## Step 2: Switch to Root User

```bash
sudo -i
```

## Step 3: Create User with Directory

```bash
useradd -u <unique id> -d <directory> -m <username>
```

## Step 4: Switch to Created User

```bash
su - <username>
```

## Step 5: Print the Directory

```bash
pwd
```