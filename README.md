# azure101
Reference material for Introduction to Cloud Computing using Microsoft Azure.

This document contains two parts:
- [Host a static website using Azure storage](#host-a-static-website-using-azure-storage)
- [Create a Linux Virtual Machine using Azure Portal](#create-a-linux-virtual-machine-using-azure-portal)

---

## Host a static website using Azure storage
1. If you don't have an Azure subscription, create a [free account](https://azure.microsoft.com/en-us/free/) before you begin.  

    **Note**: If you are a student, you can get $100 of credit to get started and sign up without a credit card [here](https://azure.microsoft.com/en-us/free/students/) by providing your school email address.

2.  [Create a GPv2 storage account](https://docs.microsoft.com/en-us/azure/storage/common/storage-quickstart-create-account?tabs=portal)

3. Using the Azure Portal, click on "Static website (preview)" under "Settings" in the left navigation bar.
<img src="https://docs.microsoft.com/en-us/azure/storage/blobs/media/storage-blob-static-website/storage-blob-static-website-portal-config.png">

4. Click "Enabled" and enter the name of the index document and (optionally) the custom error document path.

5. Upload your web assets to the "$web" container that was created as a part of static website enablement.

6. Make sure to include an index document with the name you configured. In this example, the document's name is "index.html".

    **Note**: The document name is case sensitive and therefore needs to match the name of the file in storage exactly.

7. Finally, navigate to your web endpoint to test your website.

[Reference](https://docs.microsoft.com/en-us/azure/storage/blobs/storage-blob-static-website)

---

## Create a Linux Virtual Machine using Azure Portal