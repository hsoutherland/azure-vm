<p align="center">
  <img src="https://i.imgur.com/IvCp8TH.png" height="30%" width="30%">
</p>

<h1>Creating a Virtual Machine in Microsoft Azure</h1>
In this tutorial, we will walk through how to create a Windows 10 virtual machine in Microsoft Azure. <br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)

<h2>Tutorial Outline</h2>

![image](https://github.com/user-attachments/assets/ca5138e1-0f85-4e77-9a57-19d3ab8ffff7)

<b>First</b>, log into Microsoft Azure portal. This is the home screen to the portal after the user has logged into their account. We will use this page to navigate and begin to create our virtual machine.

![image](https://github.com/user-attachments/assets/77fd8456-d4fd-4c92-aaa5-fa688e795441)

Click on <b>Virtual Machines</b>.

![image](https://github.com/user-attachments/assets/4cee3369-f9ee-4687-a8f5-f169787555dd)

After you navigate to the <b>Virtual Machines</b> page, you will see virtual machines that were previously created by the user. Since we have not created a virtual machine, there are no virtual machines to display.

![image](https://github.com/user-attachments/assets/388a1e25-9e3f-4779-9a45-4e7c573d42ea)

Under <i>Create</i>, click on <b>Azure Virtual Machine</b> to begin to create a new virtual machine within Azure.

![image](https://github.com/user-attachments/assets/72375aec-dd30-4c8e-aba7-aa3d346459b4)

Under <b>Resource Group</b>, click on <i>Create New</i> to create a new resource group. We will create a resource group called <i>VMResourceGroup</i>. For the <b>Virtual Machine Name</b>, we will name this virtual machine <i>Windows-VM</i>. Under <b>Region</b>, you can pick any region you like, but I use <i>Canada Central</i> out of preference.

![image](https://github.com/user-attachments/assets/d4fcf187-b764-4d15-abfa-19a898cc2858)

Under <b>Image</b>, since we want a virtual machine that runs the Windows 10 operating system, we will select <i>Windows 10 Pro</i>. For the <b>Size</b>, we can pick whatever we want, but I have noticed that the virtual machine works smoother and faster with at least 2 vcpus instead of the options that only provide 1 vcpu. Then, we will fill out a <b>username</b> and <b>password</b> for our virtual machine.

![image](https://github.com/user-attachments/assets/61492637-ce59-4b13-b774-ea99b0671b31)

Scroll down to the bottom and check the box under <b>Licensing</b>. You will not be able to create the virtual machine if this box is not checked. Click <b>Next: Disks</b> and then click <b>Next: Networking</b>.

![image](https://github.com/user-attachments/assets/7b203abb-e30a-4484-9790-1ae007abd32e)

On this page, we need to make sure that a virtual network and a subnet is present. We have the ability to creat a new virtual network if our heart desires, but we will stick with the one that Azure has provided for us for this tutorial. Proceed to click on <b>Review + Create</b>.

![image](https://github.com/user-attachments/assets/aaccd4fa-cdee-48ec-abd6-7f4d371f1252)

Microsoft Azure will review the information within the virtual machine that we created to see if there are any areas that we missed. Once it says "validation passed" on the top in green, then we can click on <b>Create</b> to finish building our virtual machine.

![image](https://github.com/user-attachments/assets/166f2c67-572c-4f3b-9e1a-eb966ca2a9b3)

![image](https://github.com/user-attachments/assets/de5ac17c-34e1-48d8-912c-c168fa701295)

To access our virtual machine, we need to open up <b>Remote Desktop Connection</b> under the search bar of our home computer. Once <b>Remote Desktop Connection</b> has been opened, under computer we will put the <i>Public IP Address</i> to our virtual machine in this textbox. We can find the <i>Pulbic IP Address</i> to our virtual machine by going back to the <b>Virtual Machines</b> page. We should be able to see our new virtual machine that we created (<i>Windows-VM</i>), and on the right side of the page we will find the <i>Public IP Address</i> to the virtual machine. Copy and paste the <i>Public IP Address</i> to the textbox on the <b>Remote Desktop Connection</b> application and click <b>Connect</b>.

![image](https://github.com/user-attachments/assets/7d2d58b3-8039-45a3-9291-3ed8ad6f1481)

Enter the <b>username</b> and <b>password</b> that you provided to create the virtual machine and click <b>OK</b>.

![image](https://github.com/user-attachments/assets/13e395ff-2013-4904-a327-c6e6e2810d94)

We are officially in our virtual machine!!! 👍


