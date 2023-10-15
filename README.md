![Intune Logo](https://github.com/Brandon-Baker11/Deploy-Applications-Using-Microsoft-Intune/assets/140644499/b00f0ed1-f6d2-4411-bf0c-9220ab93313b)
# Deploy-Applications-Using-Microsoft-Intune

## Environments and Technologies Used
- OracleVM VirtualBox

## Operating Systems Used
- Windows 11 (22H2)

## Deployment and Configuration Steps
In this lab we will go through the steps of deploying an app to a Windows device using Intune. These steps will include:

- Enrolling a VM to Microsoft Intune
- Configuring the apps to be deployed
- Verify the app policy after it's been deployed


The first step we will be taking is enrolling a device. I will be enrolling a Windows 11 VM running on Oracle VirtualBox. Type ***Access work or school*** in the search bar in the taskbar and select it from the best match menu.
![1](https://github.com/Brandon-Baker11/Deploy-Applications-Using-Microsoft-Intune/assets/140644499/8f29aa28-685e-42aa-9972-b4ed27489838)


From there click the blue button that says ***Connect*** at the top of the screen and then click the hyper-link that says ***Join this device to Azure Active Directory***.
Then enter your Microsoft 365 credentials.
![2](https://github.com/Brandon-Baker11/Deploy-Applications-Using-Microsoft-Intune/assets/140644499/4bb155a9-a186-440b-a6a7-e857a406db2d)


Click ***Join*** on the ***Make sure this is your organization*** pop-up window.
Then click done on the ***You're all set*** window.
![3](https://github.com/Brandon-Baker11/Deploy-Applications-Using-Microsoft-Intune/assets/140644499/4226a662-cb25-4c8a-b61a-61223ac35e22)


Next, click the account that you just connected to and select ***Info*** from the drop-down menu. From there, scroll down and click ***Sync*** located under the ***Device sync status*** section. Once it's done syncing, right-click the Windows start charm in the taskbar hover over ***Shut down or sign out*** and select ***Sign out***
![4](https://github.com/Brandon-Baker11/Deploy-Applications-Using-Microsoft-Intune/assets/140644499/e76aed5a-1507-4f78-8168-4e8a4a99e2cb)


Now, select ***Other user***, and enter your Microsoft 365 account credentials.
The first log in may take a few minutes to startup.
![5](https://github.com/Brandon-Baker11/Deploy-Applications-Using-Microsoft-Intune/assets/140644499/961dd01d-5ca2-48c7-8cd2-f8caa5b8b228)






















































































































