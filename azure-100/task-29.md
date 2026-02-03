# Azure Task 29

## Step 1: Login to Azure Portal

Login to the Azure portal.

## Step 2: Create Azure Container Registry

Search for **Azure Container Registry** and create it using the requirements provided.

## Step 3: Login to Container Registry

Login to the container registry in the Kodekloud terminal:

```bash
az acr login --name <ACR name>
```

## Step 4: Build and Push Docker Image

Navigate to the application directory:

```bash
cd pyapp
```

Build the Docker image:

```bash
docker build -t <acr login server>/<ACR repo name>:latest .
```

Push the image to the registry:

```bash
docker push <image name>
```

## Step 5: Verify Image in ACR

Check the image in the **ACR repo** section to verify it was pushed successfully.

