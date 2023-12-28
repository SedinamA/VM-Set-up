<h1>Virtual Machine Set-up</h1>
This is a brief tutorial on how to go about creating two virtual machines (VM) in Microsoft Azure.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Resource Group and Virtual Machines)


<h2>Operating Systems Used </h2>

- HP Windows 11 laptop 

<h2>Virtual Machine Creation Process </h2>

![image](https://github.com/SedinamA/VM-Set-up/assets/146953803/ffb75190-826a-4ae6-ac34-941b4c345fe9)ScreenGrab 1

The first thing we do, is set up a resource group where all the necessary elements of this lab can be located. Upon signing into the Azure subscription, navigate to the search bar and type "Resource Group" (or click (if visible) the “Resource Groups” icon on the Azure home page). The layout should resemble something similar to what's in the screengrab above. 


  
![image](https://github.com/SedinamA/VM-Set-up/assets/146953803/50942b49-7d23-4562-b579-f1b2152e36d8)ScreenGrab 2


Click on "+ Create" in the upper left corner or just click the blue "Create resource group" button on the center page 



![image](https://github.com/SedinamA/VM-Set-up/assets/146953803/0d220a55-503f-45b4-9ab3-ad866f85ab35)ScreenGrab 3


We’ll title this group “VirtM-RG” and then select a region. Then click the "Review + Create" button on the bottom left of the screen.
</p>



![image](https://github.com/SedinamA/VM-Set-up/assets/146953803/fba64adc-0484-48c6-bc38-80445fa554c1)ScreenGrab 4

Once validation is passed, click on the "Create" button



![image](https://github.com/SedinamA/VM-Set-up/assets/146953803/5995cf0d-c828-4d95-a47d-514921629342)ScreenGrab 5

Confirm that the resource group has been created (click the notification bell icon in the top right to confirm a complete creation)
<p>



![image](https://github.com/SedinamA/VM-Set-up/assets/146953803/ef07c85f-fd3b-428c-a3d8-6e027ce72424)ScreenGrab 6
 
Navigate to the search bar again and type in “virtual machine” or select the suggestion when it appears.
</p>



![image](https://github.com/SedinamA/VM-Set-up/assets/146953803/391c8962-489c-4ca4-bc9e-a526176d194e)ScreenGrab 7

In the virtual machine window, click on the icon (+ Create) in the top left corner under “Virtual Machine” and select “Azure virtual machine” on the dropdown list.



![image](https://github.com/SedinamA/VM-Set-up/assets/146953803/9186f835-a443-42ad-9f11-72ed6685e3b3)ScreenGrab 8

Use the exciting resource group(VirtM-RG) created earlier, then name the first virtual machine “VM-Windows” and make sure the selected region matches the region selected for the resource created.



![image](https://github.com/SedinamA/VM-Set-up/assets/146953803/04b8f3c5-711c-4e36-a06e-af867db4da1a)ScreenGrab 9

In the "Image" bar, we will select the type of computer we will be creating. For this computer select “Windows 10 Pro….”. For the "Size" bar, I will be selecting a standard with a size of “...-2 vcpus, 16 Gib memory….”. 



![image](https://github.com/SedinamA/VM-Set-up/assets/146953803/f5c9cc87-1461-4e9b-8e3e-af93e3131ff7)ScreenGrab 10

For the username I will be using “Windows10” and then creating a password for remote access later on (Make sure to remember the username and passwords you create). Check the box under the licensing header on the bottom left and click next. 



![image](https://github.com/SedinamA/VM-Set-up/assets/146953803/91741b8d-5d7d-48eb-b131-f29378692236)ScreenGrab 11

If you get the note in this image, just push ignore. 



![image](https://github.com/SedinamA/VM-Set-up/assets/146953803/abcea51e-c9cd-4714-b9e7-fd0cd72c1e2d)ScreenGrab 12

Click the "next" button until you arrive on the “Networking” tab.



![image](https://github.com/SedinamA/VM-Set-up/assets/146953803/251bf995-7627-4175-85bd-dcda6c094ec6)ScreenGrab 13

On this tab make note of the virtual network bar. This should be the same virtual network (VM-Windows-vnet) listed when creating the second(Ubuntu) virtual machine. Once noted, click the blue “Review + Create” button on the bottom left.



![image](https://github.com/SedinamA/VM-Set-up/assets/146953803/6ff87761-8a88-4727-800c-1603ed03fb4f)ScreenGrab 14

Once validation is passed, click the blue “Create” button in the same location(bottom left). Then click the notification bell icon in the upper right corner to verify the virtual machine has been successfully deployed. Once completed, navigate to the search bar and go to the virtual machine section, select "Azure virtual machine" once more from the "+ Create" dropdown menu (refer to ScreenGrab 7)



![image](https://github.com/SedinamA/VM-Set-up/assets/146953803/2998fb4d-3975-476a-b2e3-be887b1c9d7d)ScreenGrab 15

For the second virtual machine select the created resource group(VirtM-RG) from the dropdown, and name this machine “VM-U”. Make sure the region is the same as the resource group and Windows machine regions. 



![image](https://github.com/SedinamA/VM-Set-up/assets/146953803/dda1fe30-29df-4a62-8775-ac55d1810904)ScreenGrab 16

For the “Image” bar, select “Ubuntu Server……”. To ensure that there is a reasonable "Size" selection, I selected the same size as VM 1 (VM-Windows)



![image](https://github.com/SedinamA/VM-Set-up/assets/146953803/2281479b-8d45-4563-b9eb-9abe766a8e96)ScreenGrab 17

For authentication type, select “Password” instead of “SSH public key”. Once completed, type the username “Ubuntu” and create a password. Then navigate to the “Networking” tab. Push ignore again in the next step like you did with ScreenGrab 11.



![image](https://github.com/SedinamA/VM-Set-up/assets/146953803/dde55a0f-2cc6-47f3-92de-ac13acd172b7)ScreenGrab 18

Verify that the Virtual Network is the same as the virtual network from the first machine. If it does not show, click on the dropdown arrow in the bar to find and select the preexisting virtual network((VM-Windows-vnet) on the dropdown list. Then click “Review+create”.



![image](https://github.com/SedinamA/VM-Set-up/assets/146953803/dbe5f1e0-5d95-4c1b-aca7-daef12a6df0e)ScreenGrab 19

Once the validation process is passed, click “Create”


![image](https://github.com/SedinamA/VM-Set-up/assets/146953803/b8b0fc6f-10fb-4fa5-b147-ead938d5345c)ScreenGrab 20

Confirm that the machine has been deployed by clicking the notification bell or observing the overview screen.


![image](https://github.com/SedinamA/VM-Set-up/assets/146953803/e4a39dc3-a744-4c0d-83bf-9546e598d350)ScreenGrab 21

Navigate to the virtual machine section again and observe the status, both machines should be “running” on their respective operating systems(Linux and Windows). We have now created two virtual machines.  


*****VULNERABILITY Manag.

![image](https://github.com/SedinamA/VM-Traffic/assets/146953803/3b32603f-d4e4-49e9-a48c-a4fe096a632c)

![image](https://github.com/SedinamA/VM-Traffic/assets/146953803/bfb3b6fc-051d-431f-b154-aff5b46760dc)

![image](https://github.com/SedinamA/VM-Set-up/assets/146953803/9cd72a94-7c1e-44d6-95a8-748624f26af5)

![image](https://github.com/SedinamA/VM-Set-up/assets/146953803/55fe470d-0db0-4f64-bc3b-604d0be29fd9)

![image](https://github.com/SedinamA/VM-Set-up/assets/146953803/022a5c87-9d74-4449-a2b3-4022dafc4d77)

![image](https://github.com/SedinamA/VM-Set-up/assets/146953803/2382b5c7-5e77-479c-b98a-d9376ebb5db5)

![image](https://github.com/SedinamA/VM-Set-up/assets/146953803/68bd305d-ff88-4946-93b7-f73079979d3f)

![image](https://github.com/SedinamA/VM-Set-up/assets/146953803/e5e3210c-0e20-4ce5-9d24-b08569fe69cf)

![image](https://github.com/SedinamA/VM-Set-up/assets/146953803/4ef0aef2-a6e4-4f05-897d-93b8160144f5)

![image](https://github.com/SedinamA/VM-Set-up/assets/146953803/9f6240c6-f57b-4fae-a9d3-ffd70cc0d19f)

![image](https://github.com/SedinamA/VM-Set-up/assets/146953803/12c23696-bd2f-4911-9f4c-655bdc1ed3b5)

![image](https://github.com/SedinamA/VM-Set-up/assets/146953803/55b118c8-313f-4ca5-8558-83b3d64baaa6)

![image](https://github.com/SedinamA/VM-Set-up/assets/146953803/73735855-bdbd-4030-ba97-65ba3398adae)

![image](https://github.com/SedinamA/VM-Set-up/assets/146953803/145c8d2c-f534-4036-a6c2-00514e65fa98)

![image](https://github.com/SedinamA/VM-Set-up/assets/146953803/35ab2f55-52ad-4ecd-8049-a5a757db63cc)

![image](https://github.com/SedinamA/VM-Set-up/assets/146953803/13f38f75-5f9d-4fcc-8524-501c269bf983)

![image](https://github.com/SedinamA/VM-Set-up/assets/146953803/7f18b9f2-f7d6-4707-b68a-22b4da514b6f)












