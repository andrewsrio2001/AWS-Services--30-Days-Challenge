# AWS EC2 Setup Guide

This guide provides step-by-step instructions for launching an EC2 instance on Amazon Web Services (AWS).

## Prerequisites

- An AWS account
- AWS Management Console access

## Steps to Launch an EC2 Instance

### Step 1: Sign in to AWS Management Console
1. Go to [AWS Management Console](https://aws.amazon.com/).
2. Sign in with your AWS account credentials.

### Step 2: Open the EC2 Dashboard
1. In the top navigation bar, click on **Services**.
2. Under the **Compute** section, select **EC2**.

### Step 3: Launch an Instance
1. Click on the **Launch Instance** button.

### Step 4: Choose an Amazon Machine Image (AMI)
1. Browse the list of available AMIs.
2. Select the **Amazon Linux 2 AMI** (or another AMI as needed).
3. Click **Select**.

### Step 5: Choose an Instance Type
1. Select an instance type (e.g., **t2.micro** for free tier).
2. Click **Next: Configure Instance Details**.

### Step 6: Configure Instance Details
1. Adjust the number of instances if needed.
2. Configure network settings (default settings are usually fine).
3. Click **Next: Add Storage**.

### Step 7: Add Storage
1. Verify the default storage settings (8 GB General Purpose SSD).
2. Adjust if necessary.
3. Click **Next: Add Tags**.

### Step 8: Add Tags
1. Click **Add Tag**.
2. Enter a key-value pair (e.g., Key: Name, Value: MyEC2Instance).
3. Click **Next: Configure Security Group**.

### Step 9: Configure Security Group
1. Click **Add Rule**.
2. Set Type to **SSH** (port 22) for Linux or **RDP** (port 3389) for Windows.
3. Set Source to **My IP** to restrict access to your IP.
4. Click **Review and Launch**.

### Step 10: Review and Launch
1. Review your settings.
2. Click **Launch**.

### Step 11: Select Key Pair
1. Choose an existing key pair or create a new one.
2. Download the key pair file (.pem) and store it securely.
3. Check the acknowledgment box.
4. Click **Launch Instances**.

### Step 12: View Instances
1. Click **View Instances** to see your running instance.
2. Note the public IP address or DNS for SSH access.

## Additional Resources

- [Amazon EC2 Documentation](https://docs.aws.amazon.com/ec2/)
- [AWS Free Tier](https://aws.amazon.com/free/)
