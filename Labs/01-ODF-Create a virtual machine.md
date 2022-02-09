# 01 - Create a virtual machine in the portal (10 min)

In this walkthrough, we will create a virtual machine in the Azure portal with  the web server role installed and test. 

**Note**: Take time during this walk-through to click and read the Informational icons. 

# Task 1: Create the virtual machine 

1. Sign-in to the Azure portal: **https://portal.azure.com**

2. From the **All services** blade in the Portal Menu, search for and select **Virtual machines**, and then click **+Add, +Create, +New** and choose **+Virtual machine** from the drop down.

3. On the **Basics** tab, fill in the following information (leave the defaults for everything else):

    | Settings | Values |
    |  -- | -- |
    | Subscription | **Use default supplied** |
    | Resource group | **Create new resource group** |
    | Virtual machine name | **myVM** |
    | Region | **(US) East US**|
    | Availability options | No infrastructure redundancy options required|
    | Image | **Windows Server 2019 Datacenter - Gen2**|
    | Size | **Standard D2s v3**|
    | Administrator account username | **azureuser** |
    | Administrator account password (type in carefully!) | **Pa$$w0rd1234**|
    | Public inbound ports | **None**| 

4. Switch to the Networking tab to ensure **None** is selected in section **Public inbound ports**.

5. Switch to the Management tab, and in its **Monitoring** section, select the following setting:

    | Settings | Values |
    | -- | -- |
    | Boot diagnostics | **Disable**|


7. Leave the remaining values on the defaults and then click the **Review + create** button at the bottom of the page.

8. Once Validation has passed click the **Create** button. It can take anywhere from five to seven minutes to deploy the virtual machine.

9. You will receive updates on the deployment page and via the **Notifications** area (the bell icon in the top menu bar).

# Task 2: Confirm successful deployment of the Virtual Machine

In this task, we will confirm that to our new Virtual Machine was successfully deployed.

1. Click on bell icon from the upper blue toolbar, and select 'Go to resource' when your deployment has succeded. 

    **Note**: You could also use the **Go to resource** link on the deployment page 

2. On the virtual machine **Overview** blade, confirm that the status indicates **Running**.

**Congratulations!** You have created a new VM running in Azure. It is not yet accessible from the Internet using a public IP address. We will revisit this Virtual Machine in a later activity.
