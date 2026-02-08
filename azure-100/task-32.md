# Azure Task 32: Copy Blob Between Containers

## Step 1: Note Default Container Access

By default, all containers are private.

## Step 2: Create Destination Container

```bash
az storage container create \
	--name <> \
	--account-name <>
```

## Step 3: Copy Blob to Destination Container

```bash
az storage blob copy start \
	--source-name <> \
	--source-container <> \
	--source-blob <> \
	--destination-container <> \
	--destination-blob <>
```

## Step 4: Check Migration Status

```bash
az storage blob show \
	--account-name <> \
	--container-name <> \
	--name <> \
	--query "properties.copy.status"
```