# VM Migration: AWS EC2 to GCP Compute Engine

![AWS to GCP Migration](images/AWS%20GCP%20VM.png)

## Overview
This guide outlines the steps to migrate an EC2 instance from AWS to GCP Compute Engine using GCP's migration tools.

## Steps to Migrate

### 1. Create AWS IAM Policy
Ensure you have the necessary permissions by creating an IAM policy in AWS that allows access to the EC2 instance for migration.
Check Repo IAM-Policy file.

### 2. Initiate Migration in GCP
- Navigate to **Compute Engine** in the Google Cloud Console.
- Select **Migrate to Virtual Machine**.

![Migrate to VM](images/AWS%20GCP%20VM.png)

- Choose **AWS** as the source.

![Select AWS Source](images/AWS%20GCP%20VM.png)

### 3. Configure Source Details
- Enter the required details for the AWS source environment.
- Click **Create** after completing the configuration.

![Fill Source Details](images/AWS%20GCP%20VM.png)

### 4. Start Replication
- Under **Migrate to Virtual Machines**, go to **VM Migration**.
- Click **Start Replication** to begin data transfer from AWS to GCP.

### 5. Add Target
- Define the target environment in GCP where the VM will be hosted.

### 6. Complete Migration (Cutover)
- Once replication is complete, perform the **cutover** to finalize the migration and switch operations to GCP.

---
This guide provides a high-level overview of the migration process. For detailed instructions, refer to the [official GCP documentation](https://cloud.google.com/migrate/compute-engine/docs/).
