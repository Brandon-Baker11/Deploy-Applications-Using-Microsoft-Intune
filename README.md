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


Next, we will be creating the application deployment policy that will be used on the device that we just connected to Intune. Open Microsoft Edge and sign in to the Microsoft Intune Admin Center. Click ***Apps*** on the left hand side, then Click ***Windows*** under the ***By platform*** section.
Click ***+ Add***.
![6](https://github.com/Brandon-Baker11/Deploy-Applications-Using-Microsoft-Intune/assets/140644499/1155513a-e71c-45db-ac1d-091d121351fe)


In the fly-out window, select ***Windows 10 and later*** that is under ***Microsoft 365 apps*** and click ***Select*** 
![7](https://github.com/Brandon-Baker11/Deploy-Applications-Using-Microsoft-Intune/assets/140644499/365fcbcf-bec1-46e9-ba34-3bb1f0507759)


We can keep the defaults on the ***App suite information*** page.
Scroll down and click ***Next***
![8](https://github.com/Brandon-Baker11/Deploy-Applications-Using-Microsoft-Intune/assets/140644499/54234e66-f059-4727-852d-b87e77dfd8de)


On the ***Configure app suite*** tab, make the following changes below:
```
Default file format: Office Open Document Format
Update channel: Semi-Annual Enterprise Channel
```
Click ***Next***
![9](https://github.com/Brandon-Baker11/Deploy-Applications-Using-Microsoft-Intune/assets/140644499/e3ee0839-00ee-4b93-865d-bb7e1eedef30)


In ***Assignments*** under the ***Required*** section select ***Add all users*** and ***Add all devices***
Click ***Next***
![10](https://github.com/Brandon-Baker11/Deploy-Applications-Using-Microsoft-Intune/assets/140644499/fb086cb0-c712-45ca-829a-eae71e4bbc99)


Click ***Create*** when you get to the ***Review and create*** tab and when the policy has been created, you will be brought to the policy's overview page.
![11](https://github.com/Brandon-Baker11/Deploy-Applications-Using-Microsoft-Intune/assets/140644499/9ba80747-ce62-44c2-8a06-a0d510b2515e)


Minimize the Microsoft Edge window and we will sync our device to Intune like we did earlier in the ***Access work and school*** section in system settings.
![12](https://github.com/Brandon-Baker11/Deploy-Applications-Using-Microsoft-Intune/assets/140644499/1d54aa0b-4438-446f-a900-3912bb6326e0)


Restore the Microsoft Edge browser session and refresh application deployment overview page and you should see that there has been 1 device added to the policy.
![13](https://github.com/Brandon-Baker11/Deploy-Applications-Using-Microsoft-Intune/assets/140644499/2848f858-dff8-409c-ba19-fa879ff986ed)


Click ***Device install status*** on the left pane and you will see the device name has populated in the list of devices.
![14](https://github.com/Brandon-Baker11/Deploy-Applications-Using-Microsoft-Intune/assets/140644499/becee853-1846-4143-a518-c821ba5855c4)


Click ***User install status*** on the left pane and you will see the account that is associated with that device populated in the list.
![15](https://github.com/Brandon-Baker11/Deploy-Applications-Using-Microsoft-Intune/assets/140644499/c5e354a3-4048-48e2-94c6-d8c7f7064d94)


Now minimize the Microsoft Edge browser and type ***Word*** in the search bar located in the taskbar.
Select ***Word***
![16](https://github.com/Brandon-Baker11/Deploy-Applications-Using-Microsoft-Intune/assets/140644499/85f6c27b-4afb-4209-8e77-4eaebe4c7331)


Now you have successfully deployed an application policy onto a device using Intune!
![17](https://github.com/Brandon-Baker11/Deploy-Applications-Using-Microsoft-Intune/assets/140644499/5ef32333-e4dd-4a66-9389-689d46cc7025)






























































































