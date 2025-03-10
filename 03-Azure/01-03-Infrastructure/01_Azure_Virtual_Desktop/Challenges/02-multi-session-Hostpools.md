# Exercise 2: Multi-Session Hostpools
[Previous Challenge](./01-Personal-Hostpools.md) - **[Home](../readme.md)** - [Next Challenge](./03-Implement-FSLogix-Profile-Solution.md)

## Introduction
In this challenge you will create Azure AD DS joined pooled desktops. After deployment you will connect to the session host, deploy Notepad, 
create an Image and upload the image to the Image gallery. You will deploy a new hostpool and deploy 2 Session hosts from this image. 
Then you will provide Remote Apps to user

## Challenge
Create multi-session Hostpool joined in Azure Active Directory Domain Services
- West Europe Region
- Metadata located in West Europe
- Mark as Validation environment
- Host Pool type: Pooled
- Add 1 Virtual machine with a Windows 10 Enterprise multi-session Version 20H2 + Microsoft 365 Apps Gallery image  
- Domain to join: Azure Active Directory (Enroll with Intune “No”)
- Register desktop app group to new workspace
- Assign users

Login to the session host and create image
- Login as a user with local administrative privileges (Assign user access to Host Pools)
- Install Notepad++
- Create Image with generalized option and upload it to the shared image gallery

Deploy session host with recently created image
- Add 2 new virtual machines to the Host Pool
- Choose your recently created image
- Deploy Notepad++ as Remote App


## Success Criteria
1.	Host Pools are created and Session Hosts are showing available
2.	Users are assigned to the HostPool's appropriate app group
3.	Able to show the Host Pool settings configured.
4.	VMs are joined to Azure AD DS
5.	users can sign in to the VM.
6.	Notepad++ is installed on all VMs within the pooled Hostpool and can be accessed via RemoteApp

## Learning Resources
- [Create Azure Virtual Desktop Hostpool](https://docs.microsoft.com/de-de/azure/virtual-desktop/create-host-pools-azure-marketplace?tabs=azure-portal)
- [Capture an image of a VM using the portal](https://docs.microsoft.com/en-us/azure/virtual-machines/capture-image-portal)
- [Manage app groups for Azure Virtual Desktop portal](https://docs.microsoft.com/en-us/azure/virtual-desktop/manage-app-groups)
- [Connect with the Windows Desktop Client](https://docs.microsoft.com/en-us/azure/virtual-desktop/user-documentation/connect-windows-7-10#install-the-windows-desktop-client)








