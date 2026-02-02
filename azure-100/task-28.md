# Azure Task 28

## Step 1: Login to Azure Portal

Login to the Azure portal.

## Step 2: Configure Virtual Network

Navigate to the **VNet** section.

## Step 3: Assign Public IP

In **Network Interface** > **IP Configuration**, assign the public IP to the primary interface.

## Step 4: Configure Network Security Group

In **Network Security Group** > Create an inbound rule:
- Allow source port **80** to access Nginx

## Step 5: Attach NSG to Subnet

In **Virtual Network** > **Subnet** section, select the NSG that was already configured.

## Step 6: Configure Route Table

Navigate to **Route Table**:
- Delete the `block-internet` route
- Create a new route to access the internet

## Step 7: Reset VM Password (If Needed)

If Nginx isn't working, reset the password of the VM.

## Step 8: SSH to the VM

```bash
ssh <username>@<public_ip>
```

## Step 9: Install Nginx

```bash
sudo apt install -y nginx
```

## Step 10: Verify Installation

Check the public IP in the browser to verify Nginx is running.