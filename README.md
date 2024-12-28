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
     <br />
    <br />
     <img src="https://imgur.com/OCcYIsS.png" height="80%" width="80%" alt="Create Azure Storage Account"/>
     <br />
     <br />

### 2. Create a Storage Account
1. Navigate to **Storage accounts** and select **Create**.
2. Complete the required fields on the **Basics** page.
3. Proceed through the **Hosting** and **Monitoring** pages, configuring as needed.
4. Select **Review + Create** to deploy the storage account.
5. Use the **Notification** panel to verify deployment and access your storage account.
    <br />
    <br />
     <img src="https://imgur.com/b7RYJ2e.png" height="80%" width="80%" alt="Create Azure Storage Account"/>
     <br />
     <br />
     <img src="https://imgur.com/nXqwQL1.png" height="80%" width="80%" alt="Create Azure Storage Account"/>
     <br />
     <br />

### 3. Create an Azure Function App
1. Go to **Create a resource** and select **Compute > Function App**.
2. Fill in the details on the **Basics**, **Hosting**, and **Monitoring** pages.
3. Review your settings and select **Create** to deploy the function app.
4. Pin the function app to your dashboard for easy access.
      <br />
    <br />
     <img src="https://imgur.com/oQfcNZJ.png" height="80%" width="80%" alt="Create Azure Storage Account"/>
     <br />
     <br />
     <img src="https://imgur.com/MKb3fHn.png" height="80%" width="80%" alt="Create Azure Storage Account"/>
     <br />
     <br />

### 4. Create an Azure Blob Storage Triggered Function
1. Open your function app and navigate to **Functions**.
2. Select **+ Add**, then choose the **Azure Blob Storage trigger** template.
3. Configure the trigger settings as required and select **Create Function**.
4. Create a container for blobs:
   - Go to your storage account > **Containers** > **+ Container**.
   - Name the container `samples-workitems` and select **Create**.
  <br />
    <br />
     <img src="https://imgur.com/iqQb71B.png" height="80%" width="80%" alt="Create Azure Storage Account"/>
     <br />
     <br />
     <img src="https://imgur.com/fk5o4TG.png" height="80%" width="80%" alt="Create Azure Storage Account"/>
     <br />
     <br />
     <img src="https://imgur.com/Qru3cEV.png" height="80%" width="80%" alt="Create Azure Storage Account"/>
     <br />
     <br />

### 5. Test the Function
1. Open the function in the Azure Portal and ensure log streaming is active.
   <br />
     <img src="https://imgur.com/AXcEVJu.png" height="80%" width="80%" alt="Create Azure Storage Account"/>
     <br />
3. Upload a sample file to the `samples-workitems` container:
   - Navigate to the storage account > **Containers** > `samples-workitems`.
   - Select **Upload**, choose a file, and upload it.
     <br />
    <br />
     <img src="https://imgur.com/0XIHCAe.png" height="80%" width="80%" alt="Create Azure Storage Account"/>
     <br />
     <br />
     <img src="https://imgur.com/vepfvBP.png" height="80%" width="80%" alt="Create Azure Storage Account"/>
     <br />
     <br />

4. Verify that the blob was read by checking the function logs.
   <br />
    <br />
     <img src="https://imgur.com/sYduXYd.png" height="80%" width="80%" alt="Create Azure Storage Account"/>
     <br />
     <br />

### 6. Create an Azure SQL Database (Optional)
For advanced scenarios, integrate with an Azure SQL Database to store and process data extracted from blobs.
 <br />
    <br />
     <img src="https://imgur.com/6RVfxZ0.png" height="80%" width="80%" alt="Create Azure Storage Account"/>
     <br />
     <br />
     <img src="https://imgur.com/7o3NIsk.png" height="80%" width="80%" alt="Create Azure Storage Account"/>
     <br />
     <br />
     <img src="https://imgur.com/E4ka7zb.png" height="80%" width="80%" alt="Create Azure Storage Account"/>
     <br />
     <br />
      <img src="https://imgur.com/Yvwv6fc.png" height="80%" width="80%" alt="Create Azure Storage Account"/>
     <br />
     <br />
     <img src="https://imgur.com/wLhEjSO.png" height="80%" width="80%" alt="Create Azure Storage Account"/>
     <br />
     <br />
     <img src="https://imgur.com/nr5m74e.png" height="80%" width="80%" alt="Create Azure Storage Account"/>
     <br />
     <br />

## Contributing
Contributions are welcome! Please submit a pull request with your proposed changes.
