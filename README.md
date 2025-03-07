<p align="center">
<img src="https://github.com/user-attachments/assets/7faf52ee-ecac-4ada-bace-bab4266381eb" height="30%" width="30%"/>
</p>

<h1>Configuring Users for Active Directory</h1>
In this tutorial, we will go over how to set the Windows Server as the Domain Controller, create Administrator Account, create users and add them to Active Directory.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Virtual Network inside Azure Resource Group
- Powershell

<h2>Operating Systems Used </h2>

- Windows 10 Pro (22H2)-Client 1
- Windows Server- DC-1(Domain Controller)

<h2>Actions and Observations</h2>

<p>
<img src="https://github.com/user-attachments/assets/70f2f67d-7876-4788-9802-a6119c9efd16" height="50%" width="50%"/>

We will use the Resource group that was setup in [Creating Active Directory](https://github.com/gustygreen/Active-Directory.git) for this lab.
</p>

<h2>Install Active Directory</h2>

<p>
<img src="https://github.com/user-attachments/assets/6621188c-5143-4f2c-a3a3-e4db5ddbe786" height="50%" width="50%"/>

RDP into dc-1(Domain Controller) and install Active Directory Services in Server Manager-Add Roles and features.
</p>

<p>
<img src="https://github.com/user-attachments/assets/1545b1e9-ebb4-4c7b-a466-5992ae4ec08c" height="50%" width="50%"/>

Select Role-based or feature-based installation. Select Next
</p>

<p>
<img src="https://github.com/user-attachments/assets/98a2ce45-8486-4fbb-a9aa-61bafad4f5a2" height="50%" width="50%"/>

Leave everything defaulted. Select Next
</p>

<p>
<img src="https://github.com/user-attachments/assets/8a099abd-1e80-4417-b652-10366dda1cbf" height="50%" width="50%"/>

Check "Active Directory Domain Services". Select Next. Click Add Features
</p>

<p>
<img src="https://github.com/user-attachments/assets/2bd404b5-ae0e-4ced-8624-ca57e8b6bb43" height="50%" width="50%"/>

Select Next(3x). 
</p>

<p>
<img src="https://github.com/user-attachments/assets/67dced0f-cf2b-40ab-a64c-fddcf44375ef" height="50%" width="50%"/>

Check "Restart the destination server automatically if required. Select "Yes". Click "Install". 
</p>

<h2>Promote dc-1 to and actual Domain Controller</h2>

<p>
<img src="https://github.com/user-attachments/assets/1dbfb5c7-f223-4972-9d37-69937e0a206e" heigth="50%" width="50%"/>

On dc-1 in Server Manager, select the Flag and in the drop-down click "Promote this server to a domain controller".
</p>

<p>
<img src="https://github.com/user-attachments/assets/3703ab56-d1f8-4099-b0c1-e77b60bc563d" heigth="50%" width="50%"/>

Select "Add a new forest". Label the Root domain name. Click Next
</p>

<p>
<img src="https://github.com/user-attachments/assets/eaeba632-106d-4223-ba13-7e223eb3a774" heigth="50%" width="50%"/>

Add password. Click Next
</p>

<p>
<img src="https://github.com/user-attachments/assets/1652355e-9c91-4543-be53-e19e5d8321f4" heigth="50%" width="50%"/>

Uncheck "Create DNS delegation. Click Next
</p>

<p>
<img src="https://github.com/user-attachments/assets/1652355e-9c91-4543-be53-e19e5d8321f4" heigth="50%" width="50%"/>

Uncheck "Create DNS delegation. Click Next(3x). Click Next again on the next screen.
</p>
 
<p>
<img src="https://github.com/user-attachments/assets/d5a437ab-0521-4171-9153-5aa3d7e30f76" heigth="50%" width="50%"/>

On the Prerequisites Check screen select Install.
</p> 
After Install, the server will restart and will then be a Domain Controller.

<h2>Create an Admin in the Domain</h2>

RDP back into dc-1.

<p>
<img src="https://github.com/user-attachments/assets/d3ab6d03-e597-45d4-83ed-151531120302" height="50%" width="50%"/>

Go to Start-Windows Administrative Tools-Active Directory Users and Computers.
</p>

<p>
<img src="https://github.com/user-attachments/assets/8404c494-a206-4bc7-a5d6-1bd5d1283eb2" height="50%" width="50%"/>

Right click mydomain.com-select New-select Organizational Unit.
</p>

<p>
<img src="https://github.com/user-attachments/assets/39bb681e-51d5-44e6-8d6a-a56c3dffcbb8" height="50%" width="50%"/>

Label the new OU-_ADMINS.
</p>

<p>
<img src="https://github.com/user-attachments/assets/c408fdb8-f5a6-49da-89f6-c24f79381ce2" height="50%" width="50%"/>

Through the same process, create an OU for _EMPLOYEES as well.(This will be used in a preceeding lab.)
</p>

<h2>Add a user to _ADMINS OU</h2>
<p>
<img src="https://github.com/user-attachments/assets/3ea3c760-0513-4228-9bd0-2ca098527762" height="50%" width="50%"/>

Select the _ADMINS OU. Right click in the empty field to the right. Select New. Select User.
</p>

<p>
<img src="https://github.com/user-attachments/assets/3ea3c760-0513-4228-9bd0-2ca098527762" height="50%" width="50%"/>

Select the _ADMINS OU. Right click in the empty field to the right. Select New. Select User.
</p>


