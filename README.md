<p align="center">

![image](https://github.com/user-attachments/assets/ae645488-c16c-483a-9c3b-a5bd697e0cf1)

</p>

<h1>VPN - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation ousing a VPN.<br />

<h2>Environments and Technologies Used</h2>

- A VPN (Proton VPN)
- Microsoft Azure (Virtual Machines/Computer)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Installation Steps</h2>

1). Locate your own personal IP address by going to "www.whatismyipaddress.com" on your personal machine. This site will show your local IP address.

![image](https://github.com/user-attachments/assets/06281afa-346f-4c46-a22d-a3723fd03b36)

<p>

Next we will set up a virtual machine on Azure. 
</p>
<hr>

2). Go to www.portal.azure.com and find Virtual Machines. (You can create a free account with that comes with a $200 free credit balance). See Example 2A looking at the Virtual Machine set up page. 

<p>
<img src="https://i.imgur.com/K9oaS2z.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Creating the Virtual Machine as “VM-FranceCentral” and select that for the REGION as well. Ensure the other items are selected.

<p>
<img src="https://i.imgur.com/u3vclL3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

For the Username and Password you can create your custom information. For this example, we'll use admin_user and Cyberlab123! as the password.
  
</p>

<p>
<img src="https://i.imgur.com/rXIj3Zb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Select the “Networking” tab towards the top of the page and make sure everything is the exact same. 
  
</p>

<p>
<img src="https://i.imgur.com/OgYgNLK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Then select “Review and Create”, once it passes validation select “Create” at the bottom. 
  
</p>
<br />

Next, looking at the Virtual Machine we see that the IP to the Virtual Machine is “20.216.176.18”. 
<p>
<img src="https://i.imgur.com/ZlH9zI5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

<hr>
3). Log Into the VM and Find IP Address
<p>
Now that we have set up the Virtual Machine we will connecting to it using the application “Remote Desktop Connection” and input the IP address for the VM that we saw on Azure. Then input the login credentials when creating the VM. Once logged in, we will open the web browser and again look up www.whatismyipaddress.com on the virtual machine.

  
</p>
<br />
<p>
<img src="https://i.imgur.com/YPBkMau.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

  
</p>
<br />

<p>
<img src="https://i.imgur.com/oPJr2w2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

When we look up the IP address for this VM through www.whatismyipaddress.com we see that this VM is showing the location for France.
  
</p>
<br />

<p>
<img src="https://i.imgur.com/nWlX2UM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<hr>

4). Connecting To A VPN

Using the local computer go to protonvpn.com and create a free account (if you use the VM then French will be the language on your browser, so use the local computer desktop). Once you are logged into your account, copy the URL from the Proton VPN website and then paste the URL to the VM web browser. 

  
</p>
<br />

<p>
<img src="https://i.imgur.com/orO2O5y.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Once you have logged into your Proton VPN account on the VM, you will select “Downloads” and choose to download the “Windows” version. Once the application Proton VPN is installed we will log in using the credentials we used when setting up a free account on Proton VPN. Then connect to the VPN through the installed app. 
  
</p>
<br />


<p>
<img src="https://i.imgur.com/oqPHozb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

On the left hand side of the VPN you can select a country where you want your VPN to be, the image below shows the VPN being connected to an IP in Japan.
  
</p>
<br />

<p>
<img src="https://i.imgur.com/6Rdgg6B.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Next we will look at the IP again using the VM browser now that we have connected the VPN to Japan. The website www.whatismyipaddress.com shows yet another IP address using the VPN from Japan. This is quite amazing.
  
</p>
<br />

<p>
<img src="https://i.imgur.com/lQsISWb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Looking at this exercise we see that we have utilized 3 different IP addresses just from your local computer to connect to the internet.
Home IP (USA): 137.103.51.136
Virtual Machin IP (France): 20.216.176.18
Virtual Machin IP VPN (Japan) 212.102.51.251

  
</p>
<br />

Congratulations you have successfully set up a VPN on a virtual machine through this tutorial.
