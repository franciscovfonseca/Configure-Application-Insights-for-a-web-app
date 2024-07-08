<br>

<p align="center">
<img width="500" src="https://github.com/franciscovfonseca/Configure-Virtual-Network-Connectivity-by-Using-Peering/assets/172988970/5795419a-3012-4a57-b4b0-155c2dd93fc7" alt="Microsoft Active Directory Logo"/>
<br>
<br>
<br>



<h1> Configure Application Insights for a Web App</h1>
<br>

In this exercise, you will configure Application Insights for a web app by using the Azure portal.

1. First, you will create a web app.

2. Next, you will deploy ASP.NET code to the web app.

3. Finally, you will configure and test Application Insights.
<br>

You can use the Azure App Service to host your web apps in the cloud in a fully managed environment.

You can deploy your own code by using the programming language of your choice and the tools you are familiar with.

As part of your security strategy, you can monitor usage of your web app by using Application Insights.


<br>
<br>

<h2>1️⃣ Create a Web App</h2>
<br>

In this task, you will use the Azure portal to create a web app, and then you will test the app by using its public URL.

<br>

✅ If necessary, sign in to Windows 10 - RDP Jumpbox as LabUser using Passw0rd! as the password.

- 💡 Select the Type Text icon to type the associated text into the virtual machine at the current cursor location.
<br>

<br>

✅ Open Microsoft Edge, and then sign in to http://portal.azure.com as admin-42241754@cloudslice.onmicrosoft.com using cDeC3e!0D@ as the password.

- If you receive an error, select Try again.
<br>

<br>

✅ If prompted to take a tour of the Azure portal, select Maybe later.

<br>

✅ In the Azure portal, in the upper-left corner, select the Show portal menu icon.
<p align="center">
<img src="https://github.com/franciscovfonseca/Configure-Virtual-Network-Connectivity-by-Using-Peering/assets/172988970/5b9a2405-7215-4592-95f3-363c871949ef" height="80%" width="80%" alt="9"/><br />
<br>

<br>

✅ On the Azure portal menu, select Create a resource to display the Azure Marketplace.

<br>

✅ In the Popular Azure services list, select Web App.

<br>

✅ On the Create Web App blade, on the Basics page, in Resource Group, select corp-datalod42241754, and then in Name, enter web42241754.

<br>

✅ In Publish, ensure that Code is selected, in Runtime stack, select ASP.NET V4.8 (or the most recent version), in Operating System, ensure that Windows is selected, and then in Region, select East US.

<br>

✅ In App Service Plan, in Sku and size, select Explore pricing plans.

<br>

✅ On the Select App Service Pricing Plan blade, locate and select Standard S1, and then select Select.
<p align="center">
<img src="https://github.com/franciscovfonseca/Configure-Virtual-Network-Connectivity-by-Using-Peering/assets/172988970/5b9a2405-7215-4592-95f3-363c871949ef" height="80%" width="80%" alt="9"/><br />
<br>

<br>

✅ On the Basics page, select Next: Database, and then select Next : Deployment.

<br>

✅ On the Deployment page, in Continuous deployment settings, ensure that Disable is selected, and then select Next : Networking.

- You will deploy code for the web app in an upcoming task.
<br>

<br>

✅ On the Networking page, in Enable network injection, ensure that Off is selected, and then select Next : Monitoring.

<br>

✅ On the Monitoring page, in Enable Application Insights, ensure that No is selected.

- You will enable Application Insights in an upcoming task.
<br>

<br>

✅ Select Review + create, review the configuration, and then select Create to deploy the web app.

- The web app deployment will take approximately 1–2 minutes to complete.
<br>

<br>

✅ When you are presented with a Your deployment is complete message, select Go to resource to display the web42241754 page.
<p align="center">
<img src="https://github.com/franciscovfonseca/Configure-Virtual-Network-Connectivity-by-Using-Peering/assets/172988970/5b9a2405-7215-4592-95f3-363c871949ef" height="80%" width="80%" alt="9"/><br />
<br>

<br>

✅ On the web42241754 page, select the URL link to test the deployment.

- You should see the default home page of the web app.
<p align="center">
<img src="https://github.com/franciscovfonseca/Configure-Virtual-Network-Connectivity-by-Using-Peering/assets/172988970/5b9a2405-7215-4592-95f3-363c871949ef" height="80%" width="80%" alt="9"/><br />
<br>

<br>

✅ Close the browser window that contains default home page of the web app.

<br>
<br>

<h2>2️⃣ Deploy ASP.NET Code</h2>
<br>

In this task, you will deploy ASP.NET code to your web app, and then you will test the updated app by using the public URL of the web app.

<br>

✅ On the web42241754 resource menu, in Deployment, select Deployment Center.

<br>

✅ On the Deployment Center page, on the Settings page, select SCM basic authentication is disabled for your app. Click here to go to your configuration settings to enable.
<p align="center">
<img src="https://github.com/franciscovfonseca/Configure-Virtual-Network-Connectivity-by-Using-Peering/assets/172988970/5b9a2405-7215-4592-95f3-363c871949ef" height="80%" width="80%" alt="9"/><br />
<br>

<br>

✅ On the Configuration blade, in Platform settings, in SCM Basic Auth Publishing Credentials, select On, and then on the command bar, select Save.

<br>

✅ On the Save changes blade, select Continue, and then close the Configuration blade.

<br>

✅ On the Deployment Center page, on the Settings page, in Source, select External Git.
<p align="center">
<img src="https://github.com/franciscovfonseca/Configure-Virtual-Network-Connectivity-by-Using-Peering/assets/172988970/5b9a2405-7215-4592-95f3-363c871949ef" height="80%" width="80%" alt="9"/><br />
<br>

<br>

✅ In External Git, in Repository, enter https://github.com/LODSContent/LODSOC_app-service-web-dotnet-get-started, in Branch, enter main, and then in Repository Type, ensure that Public is selected.
<p align="center">
<img src="https://github.com/franciscovfonseca/Configure-Virtual-Network-Connectivity-by-Using-Peering/assets/172988970/5b9a2405-7215-4592-95f3-363c871949ef" height="80%" width="80%" alt="9"/><br />
<br>

<br>

✅ On the command bar, select Save to initiate the deployment.

- It will take approximately 1–2 minutes for the new code to fully deploy.
<br>

<br>

✅ On the web42241754 resource menu, select Overview, and then select the URL link to display the updated version of the web app.
<p align="center">
<img src="https://github.com/franciscovfonseca/Configure-Virtual-Network-Connectivity-by-Using-Peering/assets/172988970/5b9a2405-7215-4592-95f3-363c871949ef" height="80%" width="80%" alt="9"/><br />

- If you do not see the updated page, refresh the browser.
<br>

<br>

✅ Close the browser window that contains the updated ASP.NET home page.

<br>
<br>




<br>
<br>
<br>
<br>
<br>

On the Azure portal home page, select **Create a resource** to display the Azure Marketplace.
<p align="center">
<img src="https://github.com/franciscovfonseca/Configure-Virtual-Network-Connectivity-by-Using-Peering/assets/172988970/5b9a2405-7215-4592-95f3-363c871949ef" height="80%" width="80%" alt="9"/><br />
<br>

In Search the Marketplace, search for and select ***Virtual Network***, and then select **Create**.
<p align="center">
<img src="https://github.com/franciscovfonseca/Configure-Virtual-Network-Connectivity-by-Using-Peering/assets/172988970/d5bede9d-9732-4c85-8d17-af609b9726fa" height="80%" width="80%" alt="9"/><br />
<br>
  
<p align="center">
<img src="https://github.com/franciscovfonseca/Configure-Virtual-Network-Connectivity-by-Using-Peering/assets/172988970/ca90a091-571d-49f1-beed-ddd25755c5c9" height="80%" width="80%" alt="9"/><br />
<br>

On the Create virtual network blade, on the Basics page, in Resource group, select **corp-datalod42226775**, in Virtual network name, enter ***webVNET***, and then select **Next**.
<p align="center">
<img src="https://github.com/franciscovfonseca/Configure-Virtual-Network-Connectivity-by-Using-Peering/assets/172988970/e1696f0a-06fd-4ae4-ae95-3f6c8bfd0507" height="50%" width="50%" alt="9"/><br />
<br>

On the Security page, select **Next**.

On the IP addresses page, in IPv4 address space, select **Delete address space**, and then select **Add IPv4 address space**.
<p align="center">
<img src="https://github.com/franciscovfonseca/Configure-Virtual-Network-Connectivity-by-Using-Peering/assets/172988970/c0524a5f-97cb-478a-bad8-b6fc9236fe7f" height="50%" width="50%" alt="9"/><br />
<br>

For IP address, enter ***10.10.0.0***, and confirm the subnet mask is **/16**.

Select **Add a subnet** to open the Add subnet blade.
<p align="center">
<img src="https://github.com/franciscovfonseca/Configure-Virtual-Network-Connectivity-by-Using-Peering/assets/172988970/aa430c55-3c00-4b97-b21a-aa572a0f2373" height="50%" width="50%" alt="9"/><br />
<br>

On the Add subnet blade, in Subnet name, enter ***web***, in Starting address, enter ***10.10.0.0***.

In Subnet size, select **/25**, and then select **Add**.
<p align="center">
<img src="https://github.com/franciscovfonseca/Configure-Virtual-Network-Connectivity-by-Using-Peering/assets/172988970/9b7da0cd-748d-4bb3-a77b-c12abd46eb7a" height="50%" width="50%" alt="9"/><br />
<br>

On the Create virtual network blade, select **Review + create**, and then select **Create** to create the virtual network.
<p align="center">
<img src="https://github.com/franciscovfonseca/Configure-Virtual-Network-Connectivity-by-Using-Peering/assets/172988970/f75b053a-1f8a-4b33-b502-73fa7feba6b3" height="50%" width="50%" alt="9"/><br />
<br>

✅ You will use this **Virtual Network** for the **Web Tier**.

<br>
<br>

<h2>2️⃣ Create a Virtual Network by using Azure Cloud Shell</h2>
<br>
 
In the Azure Portal, in the global controls, select the **Cloud Shell** icon.
<p align="center">
<img src="https://github.com/franciscovfonseca/Configure-Virtual-Network-Connectivity-by-Using-Peering/assets/172988970/83d5df37-6cdb-4da2-8fa9-99a4fdb61607" height="80%" width="80%" alt="9"/><br />
<br>

In the Welcome to Azure Cloud Shell dialog box, select **Bash**.
<p align="center">
<img src="https://github.com/franciscovfonseca/Configure-Virtual-Network-Connectivity-by-Using-Peering/assets/172988970/56b65cb6-9732-45a0-abbe-ab0bdd5557d0" height="80%" width="80%" alt="9"/><br />
<br>

In the Getting started window, select **Mount storage account**, in Storage account subscription, select the existing **hallenge Labs** option, and then select **Apply**.
<p align="center">
<img src="https://github.com/franciscovfonseca/Configure-Virtual-Network-Connectivity-by-Using-Peering/assets/172988970/598c5ba9-9345-4c4a-9c3f-602c8ed9c580" height="80%" width="80%" alt="9"/><br />
<br>

In the Mount storage account window, select **I want to create a storage account**, and then select **Next**.
<p align="center">
<img src="https://github.com/franciscovfonseca/Configure-Virtual-Network-Connectivity-by-Using-Peering/assets/172988970/03d7e688-f940-451a-873f-c601cb059b02" height="80%" width="80%" alt="9"/><br />
<br>

In the Create storage account window, in Resource group, select **corp-datalod42226775**.

In Region, select **(US) East US**.

In Storage account name, enter ***cs42226775***.

In File share, enter ***cloudshell***, and then select **Create**.
<p align="center">
<img src="https://github.com/franciscovfonseca/Configure-Virtual-Network-Connectivity-by-Using-Peering/assets/172988970/81b26701-7e3a-4e31-96d1-ac2481276ecc" height="80%" width="80%" alt="9"/><br />
<br>

The Cloud Shell should take approximately 1–2 minutes to initialize.


✅ You will use this **Virtual Network** for the **Application Tier**.

<br>
<h2></h2>
<br>

In Azure Cloud Shell, run the following command to create a virtual network and subnet:

```commandline
az network vnet create --name appVNET --resource-group corp-datalod42226775 --address-prefix 10.20.0.0/16 --subnet-name app --subnet-prefix 10.20.0.0/25
```
<br>

⚠️ Cloud Shell does not support the keyboard shortcut Ctrl+V for paste.

- Instead, select the command prompt, and then use **Ctrl+Shift+V** to paste.

<p align="center">
<img src="https://github.com/franciscovfonseca/Configure-Virtual-Network-Connectivity-by-Using-Peering/assets/172988970/1633eed3-851a-4949-9c7e-f920217d3425" height="80%" width="80%" alt="9"/><br />
<br>

<p align="center">
<img src="https://github.com/franciscovfonseca/Configure-Virtual-Network-Connectivity-by-Using-Peering/assets/172988970/eb66d335-b144-46bb-8adc-59ff15426181" height="80%" width="80%" alt="9"/><br />
<br>
<h2></h2>
<br>

Run the following command to verify the presence of a virtual network and subnet:

```commandline
az network vnet show --name appVNET --resource-group corp-datalod42226775
```
<br>
<p align="center">
<img src="https://github.com/franciscovfonseca/Configure-Virtual-Network-Connectivity-by-Using-Peering/assets/172988970/ce8116a3-778c-4113-abae-66448f272a19" height="80%" width="80%" alt="9"/><br />
<br>

The following screenshot shows the virtual network name and subnet name property values in the command output:
<p align="center">
<img src="https://github.com/franciscovfonseca/Configure-Virtual-Network-Connectivity-by-Using-Peering/assets/172988970/dd402600-f67e-4a8b-8f94-c5d917f0d207" height="80%" width="80%" alt="9"/><br />
<br>

Close the **Cloud Shell** window.

<br>
<br>

<h2>3️⃣ Configure Peering Connections between the Virtual Networks</h2>
<br>
 
On the Azure portal home page, in the Search bar, search for and select webVNET to display the ***webVNET*** virtual network page.
<p align="center">
<img src="https://github.com/franciscovfonseca/Configure-Virtual-Network-Connectivity-by-Using-Peering/assets/172988970/516d697e-5e68-4355-bc73-59c724b948ca" height="80%" width="80%" alt="9"/><br />
<br>

On the webVNET resource menu, in Settings, select **Peerings**.
<p align="center">
<img src="https://github.com/franciscovfonseca/Configure-Virtual-Network-Connectivity-by-Using-Peering/assets/172988970/d963ab25-143b-4ed2-973b-dab7bfe2c1ac" height="50%" width="50%" alt="9"/><br />
<br>

Then on the command bar, select **Add** to add a peering connection between the virtual networks.
<p align="center">
<img src="https://github.com/franciscovfonseca/Configure-Virtual-Network-Connectivity-by-Using-Peering/assets/172988970/d3d74ed6-9eec-47ff-a1f3-98ed6d7043f9" height="50%" width="50%" alt="9"/><br />
<br>

On the Add peering page, in This virtual network, in Peering link name, enter ***webVNET-to-appVNET***.

In Remote virtual network, in Peering link name, enter ***appVNET-to-webVNET***, and then in Virtual network, select **appVNET**.

Select **Add**, and then wait for the peering connection to be created.
<p align="center">
<img src="https://github.com/franciscovfonseca/Configure-Virtual-Network-Connectivity-by-Using-Peering/assets/172988970/fc27650f-9247-49a3-ac51-64ef679bb683" height="50%" width="50%" alt="9"/><br />

<br>
<h2></h2>
<br>

<h3>➡️ Verify that the webVNET-to-appVNET peering connection status is Connected</h3>
<br>

On the webVNET resource menu, in Settings, select **Peerings**.

On the Peerings page, in webVNET-to-appVNET, verify that the Peering status is **Connected**.

<p align="center">
<img src="https://github.com/franciscovfonseca/Configure-Virtual-Network-Connectivity-by-Using-Peering/assets/172988970/cf3a2150-bd07-4114-b14e-73d709c1f447" height="80%" width="80%" alt="9"/><br />

 <br>
<h2></h2>
<br>

<h3>➡️ Verify that the appVNET-to-webVNET peering connection status is Connected</h3>
<br>

On the webVNET - Peerings page, in webVNET-to-appVNET, in Peer, select **appVNET** to display the appVNET virtual network page.

<p align="center">
<img src="https://github.com/franciscovfonseca/Configure-Virtual-Network-Connectivity-by-Using-Peering/assets/172988970/1342638a-bf12-444a-bf09-7895103fb32e" height="80%" width="80%" alt="9"/><br />
<br>

On the appVNET resource menu, in Settings, select **Peerings**.

<p align="center">
<img src="https://github.com/franciscovfonseca/Configure-Virtual-Network-Connectivity-by-Using-Peering/assets/172988970/acf4fa7d-33c0-4f57-a5f1-3217d117028b" height="50%" width="50%" alt="9"/><br />
<br>

On the Peerings page, in appVNET-to-webVNET, verify that the Peering status is **Connected**.

<p align="center">
<img src="https://github.com/franciscovfonseca/Configure-Virtual-Network-Connectivity-by-Using-Peering/assets/172988970/60a8e0eb-b7ff-4b1d-a27a-bdd503f3d5a9" height="80%" width="80%" alt="9"/><br />
<br>

If the peering connection does not appear on the Peerings page, on the command bar, select **Refresh**.

<br>
<br>

<h2>Summary</h2>

Congratulations, you have completed the **Configure Virtual Network Connectivity by using Peering** Lab.

You have accomplished the following:

- Created a **Virtual Network for a Web Server Tier** by using the **Azure Portal**.

- Created a **Virtual Network for an Application Server Tier** by using **Azure CLI commands in Azure Cloud Shell**.

- Configured **Peering Connections** between the **Virtual Networks**.

<br>
<br>
<br>
<br>
