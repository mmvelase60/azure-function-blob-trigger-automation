# Azure Blob File Processing with Blob Trigger

This repository demonstrates how to process blob files automatically using an Azure Function with a Blob Trigger. The project includes step-by-step instructions to set up the necessary Azure resources, create and configure the Azure Function, and test the functionality.

## Features
- Automate blob file processing with Azure Functions.
- Set up resource groups, storage accounts, and function apps in Azure.
- Configure Azure Blob Storage triggers for real-time file handling.
- Test the solution with sample blob uploads.
- Integrate with an Azure SQL Database for further processing.

## Setup Instructions

### 1. Create a Resource Group
1. Sign in to the [Azure Portal](https://portal.azure.com/).
2. Navigate to **Resource groups** and select **Add**.
3. Fill in the required details:
   - **Subscription**: Select your Azure subscription.
   - **Resource group**: Provide a unique name for your resource group.
   - **Region**: Choose an Azure location.
4. Select **Review + Create**, then **Create**.
5. Refresh the resource group list or use the **Notification** bell to locate the newly created resource group.

### 2. Create a Storage Account
1. Navigate to **Storage accounts** and select **Create**.
2. Complete the required fields on the **Basics** page.
3. Proceed through the **Hosting** and **Monitoring** pages, configuring as needed.
4. Select **Review + Create** to deploy the storage account.
5. Use the **Notification** panel to verify deployment and access your storage account.

### 3. Create an Azure Function App
1. Go to **Create a resource** and select **Compute > Function App**.
2. Fill in the details on the **Basics**, **Hosting**, and **Monitoring** pages.
3. Review your settings and select **Create** to deploy the function app.
4. Pin the function app to your dashboard for easy access.

### 4. Create an Azure Blob Storage Triggered Function
1. Open your function app and navigate to **Functions**.
2. Select **+ Add**, then choose the **Azure Blob Storage trigger** template.
3. Configure the trigger settings as required and select **Create Function**.
4. Create a container for blobs:
   - Go to your storage account > **Containers** > **+ Container**.
   - Name the container `samples-workitems` and select **Create**.

### 5. Test the Function
1. Open the function in the Azure Portal and ensure log streaming is active.
2. Upload a sample file to the `samples-workitems` container:
   - Navigate to the storage account > **Containers** > `samples-workitems`.
   - Select **Upload**, choose a file, and upload it.
3. Verify that the blob was read by checking the function logs.

### 6. Create an Azure SQL Database (Optional)
For advanced scenarios, integrate with an Azure SQL Database to store and process data extracted from blobs.

## Contributing
Contributions are welcome! Please submit a pull request with your proposed changes.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
