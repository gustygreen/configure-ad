<p align="center">
<img src="https://github.com/user-attachments/assets/26c221f8-27dc-488e-a563-bdf1e63ea7a1" height="30%" width="30%"/>
</p>

<h1>Creating Azure Virtual Machines</h1>
In this tutorial, we will go over how to create VMs for Windows and Linux that will be used for the preceeding Labs.<br />


<h2>Create a Resource Group</h2>
<p>
<img src="https://github.com/user-attachments/assets/6544549a-dfd3-4a61-91c4-2ff1743f89ad" heigth="80%" width="80%"/>
<p>
Select Resource groups.
</p>
<p>
___________________________________________________________________________________________________________________________
</p>

<p>
<img src="https://github.com/user-attachments/assets/5a75f6e2-067a-4670-b912-1b80b134c024" heigth="80%" width="80%"/>
</p>
Name the Resource Group. Select a Region for the Resource Group. Review and create.
<p>
___________________________________________________________________________________________________________________________
</p>

<p>
<img src="https://github.com/user-attachments/assets/1a66f392-59a7-4eff-9773-b3c715516847" heigth="50%" width="50%"/>
</p>
Select Create.
<p>
___________________________________________________________________________________________________________________________
</p>

<h2>Create a Windows Virtual Machine</h2>
<p>
<img src="https://github.com/user-attachments/assets/f2939fa4-17b0-4c13-aad5-8871ed36eeb6" heigth="50%" width="50%"/>
</p>
Create the Virtual Machines by selecting the resource-Virtual Machine. (There are numerous ways in Azure to select it.)
<p>
___________________________________________________________________________________________________________________________
</p>

<p>
<img src="https://github.com/user-attachments/assets/63e26ca1-57f5-4add-a697-98613e3763f8" heigth="50%" width="50%"/>
</p>
Select Create and Azure virtual machine.
<p>
___________________________________________________________________________________________________________________________
</p>

<p>
<img src="https://github.com/user-attachments/assets/43087805-5e3c-42d6-8723-636ef8639573" heigth="50%" width="50%"/>
</p>
Select the Resource Group. Name the Virtual Machine and select the same region as the Resource Group for the VM.
<p>
___________________________________________________________________________________________________________________________
</p>

<p>
<img src="https://github.com/user-attachments/assets/d0d70ea4-35f2-4d79-99ec-2423d36e12dc" heigth="50%" width="50%"/>
</p>
Select the Available Zone(1) that has the size of hardware available to use(3). Select the Image(2) for the type of VM that is being created.
<p>
___________________________________________________________________________________________________________________________
</p>

<p>
<img src="https://github.com/user-attachments/assets/fc88ab6a-386f-4b5a-af8c-cc1affefb117" heigth="50%" width="50%"/>
</p>
Create a User Name(1). Create and Confirm a password(2). With Windows 10 being selected, check the Licensing field(3). Review and Create(4).
<p>
___________________________________________________________________________________________________________________________
</p>

<p>
<img src="https://github.com/user-attachments/assets/55acfb64-13d2-49d7-bac4-81d222d7f5e0" heigth="50%" width="50%"/>
</p>
After Validation has passed, select Create.
<p>
___________________________________________________________________________________________________________________________
</p>


<h2>Create a Linux(Ubuntu) Virtual Machine</h2>

<p>
<img src="https://github.com/user-attachments/assets/31350b10-ffb3-4fed-8a71-e096aa0d94c1" heigth="50%" width="50%"/>
</p>
Follow the same process as creating the Windows VM. Name the machine, make sure it's in the same Region. Select an Ubuntu Server Image.
<p>
___________________________________________________________________________________________________________________________
</p>

<p>
<img src="https://github.com/user-attachments/assets/503d3721-7540-4054-9bf3-fbeb804d381c" heigth="50%" width="50%"/>
</p>
Select the Server size. Change Authenticate Type to Password. Assign a Username and Password. Review and Create.
<p>
___________________________________________________________________________________________________________________________
</p>

<p>
<img src="https://github.com/user-attachments/assets/05801e58-8762-41e6-a78f-bce7be0352d6" heigth="50%" width="50%"/>
</p>
After Validation has passed, select Create.
<p>
___________________________________________________________________________________________________________________________
</p>

<h2>View the newly created Virtual Machines in the Resource Group.</h2>
<p>
<img src="https://github.com/user-attachments/assets/595a56e2-764a-47f8-bfd3-f0d4acce4a33" heigth="50%" width="50%"/>
</p>
After the deployment is complete there should now be 2 VMs listed under the Resource Group. 
<p>

<p>
This completes  the process of adding Virtual Machines in Azure.
</p>
