<h1>Active-Directory</h1> 
<h2>Description</h2>
<h3>This lab is a walkthrough of creating an Active Directory that I followed through [Josh Madakor](https://www.youtube.com/watch?v=MHsI8hJmggI&t=3329s). The purpose of this lab is to get an understanding of how an Active </h3>
<br />

<h2>Languages and Utilities Used</h2>
<h2>Environments Used</h2>
<br/>

<h2>Downloading Virtual Box, Windows Server 2019, and Windows 10 ISO</h2>
<img src="https://i.imgur.com/1xQCTEN.png" height="80%" width="100%"/>
- <b>Download and install Virtual Box "Window Hosts" and then "All supported platforms" from this URL "[https://www.virtualbox.org/wiki/Downloads]".<br>
<img src="https://i.imgur.com/Kl8NqzY.png" height="80%" width="100%"/>
- <b>Install Windows Server 2019 ISO "[https://www.microsoft.com/en-us/evalcenter/download-windows-server-2019] that will be used for the Virtual Box.<br>
<img src="https://i.imgur.com/7ay0JFL.png" height="80%" width="100%"/>
- <b>Lastly download Windows 10 ISO "[https://www.microsoft.com/en-us/software-download/windows10]" that will be used near the end of the lab.<br>
<br/>

<h2>Setting up the Virtual Machine</h2>
<img src="https://i.imgur.com/B21pIcX.png" height="80%" width="100%"/>
- <b>Create any name for your Virtual Box ("DomainController" since this is the purpose of this Virtual Machine) and use version "Other Windows (64-bit).<br>
<br/>
<img src="https://i.imgur.com/vbnK6JV.png" height="80%" width="100%"/>
- <b>Set the RAM and CPU that your PC/laptop can manage comfortably.<br>
<br/>
<img src="https://i.imgur.com/o7xWmOa.png" height="80%" width="100%"/>
- <b>Hit "Next."<br>
<br/>
<img src="https://i.imgur.com/StoMfHz.png" height="80%" width="100%"/>
- <b>After overviewing the Machine Name, Machine Folder, Guest OS Type, RAM, and CPU; hit "Finish."<br>
<br/>
<img src="https://i.imgur.com/d8JS6Xa.png" height="80%" width="100%"/>
- <b>The Virtual Box is setup, but navigate to "Settings (Purple Box)"<br>
<br/>
<img src="https://i.imgur.com/v3aiH6X.png" height="80%" width="100%"/>
- <b>Navigate to the "Advanced" tab and adjust the "Shared Clipboard" and "Drag'n'Drop" to both Bidirectional.<br>
- <b>This essentially allows the user to work as well as move files in and out of the Virtual Machine and your Desktop.<br>
<br/>
<img src="https://i.imgur.com/IaxcwxU.png" height="80%" width="100%"/>
<img src="https://i.imgur.com/gOIgEZI.png" height="80%" width="100%"/>
- <b>Navigate to the "Network" tab, change "Adapter 1" to "NAT," "Adapter 2" to "Internal Network," press OK, and double click the Virtual Box (DomainController) to begin running the software.<br>
- <b>Adapter 1 is being connected to the internet externally while Adapter 2 is connected internally which are conjoined by a DomainController (Windows 2019 ISO). Companies or schools, for example, would have Adapter 2 (in this case) to control certain actions/regulations for security measures on their internal networks. <br>
<br/>

<h2>Running Windows 2019 ISO on the Virtual Machine/Box</h2>
<img src="https://i.imgur.com/NdyVtlP.png" height="80%" width="100%"/>
<img src="https://i.imgur.com/CCjcZon.png" height="80%" width="100%"/>
- <b>Select the "DVD" and click the Windows 2019 ISO file that was downloaded in the beginning.<br>
- <b>Click "Mount and Retry Boot," and this will take a period of time to setup until you reach the next image below. </b>
<br>
<img src="https://i.imgur.com/BOAILjw.png" height="80%" width="100%"/>
<img src="https://i.imgur.com/bV2arW3.png" height="80%" width="100%"/>
- <b>Choose your preferred language and then "Install"<br>
- <b>The next additional steps press "next" or click on the Red box as demonstrated on the upcoming images.<br>
<br/>
<img src="https://i.imgur.com/JYJXWy4.png" height="80%" width="100%"/>
<img src="https://i.imgur.com/A6pa67A.png" height="80%" width="100%"/>
<img src="https://i.imgur.com/dEs7CLe.png" height="80%" width="100%"/>
<img src="https://i.imgur.com/7zPiG3o.png" height="80%" width="100%"/>
- <b>After this step, it's going to take a period of time for the Windows to install and it's going to restart itself. During the process DO NOT press any keys until you are at the next step (image below).<br>
<br/>

<h2>Creating a password and logging into the Virtual Box</h2>
<img src="https://i.imgur.com/ziNQxJY.png" height="80%" width="100%"/>
- <b>Create any desired password that you'll remember (I used "Password1").<br>
<br/>
<img src="https://i.imgur.com/DReJl9Q.png" height="80%" width="100%"/>
- <b>Since you cannot type the key "Ctrl+Alt+Delete", you're going to have to use the 
  Input->Keyboard->Insert Ctrl+Alt+Delete.<br>
<br/>
<img src="https://i.imgur.com/dfHQn4J.png" height="80%" width="100%"/>
- <b>Type the password that you created (Password1).<br>
<img src="https://i.imgur.com/CkmxJuQ.png" height="80%" width="100%"/>
- <b>To allow autoadjusting resolution to the window and a smooth mouse movement, (RED BOX) use the drop down menu and click on "Insert Guest Additions CD Image..."<br>
- <b>Navigate through the red boxes as shown in the next two images until you reach a pop-up window, then follow the steps to Install and lastly reboot.<br>
<img src="https://i.imgur.com/W2TEYMy.png" height="80%" width="100%"/>
<img src="https://i.imgur.com/YMYg8iM.png" height="80%" width="100%"/>
- <b>Your screen should look like the image as shown below.<br>
<img src="https://i.imgur.com/hzRpHkv.png" height="80%" width="100%"/>
<br/>
<br/>

<h2>Internal and External Networks of the Virtual Box</h2>
<img src="https://i.imgur.com/6ug0546.png" height="80%" width="100%"/>
- <b>Navigate to the network settings on the Virtual Box and click on "Change adapter options"<br>
<br/>
<img src="https://i.imgur.com/L04Grun.png" height="80%" width="100%"/>
- <b>There are two options of Ethernet Networks. (RED) From Ethernet -> Details... -> IPv4 Address, based on the IPv4 address one can identify that it's the external network (network connected to the internet or "Adapter 1").<br>
<br/>
<img src="https://i.imgur.com/xwqiQa4.png" height="80%" width="100%"/>
- <b>(ORANGE BOX) Since we know which is the external and internal networks, we renamed them ("Xx_Internet_xX" and "l_INTERNAL_l") to sort them out easier.<br>
- <b>(RED BOX) Looking into the IPv4 Address from the internal network, note that it has an "Autoconfiguration" because "Adapter 2" was unable to find a DCHP server thus it was auto-assigned a IP address. <br>
<br/>
<img src="https://i.imgur.com/hYK4AHN.png" height="80%" width="100%"/>
- <b>This step is assigning an IP address for our Internal Network, thus insert the addresses as show above and press "OK" for all.<br>
- <b>A default gateway is not entered because the Domain Controller (Windows 2019 ISO) is going to serve as the default gateway to the External Network (the internet)<br>
- <b>The "Preferred DNS server" address 127.0.0.1 is a common loopback address to ping itself as the DNS server, but using the same IP address 172.16.0.1 serves the same effect as well.<br>
<br/>

<h2>Renaming the PC to "DomainControllerPC"</h2>
<img src="https://i.imgur.com/zcCzN7g.png" height="80%" width="100%"/>
- <b>Renaming the PC is helpful for other users/admins to detect and sort between multiple PCs and generally is a good practice to perform ahead of time.<br>
<br/>

<h2>Installing Active Directory Domain Services(AD DS)</h2>
<img src="https://i.imgur.com/ujXzbc0.png" height="80%" width="100%"/>
<img src="https://i.imgur.com/w3VWsIs.png" height="80%" width="100%"/>
- <b>Nagivate thorugh the "Server Manager - Dashboard" by clicking "Add roles and features"<br>
- <b>A pop-up window appears and press "Next" until arriving at the "Server Selection" tab.<br>
- <b>Currently there's only one server available to be selected to install AD DS, then hit "Next".<br>
<br/>
<img src="https://i.imgur.com/pJnBukt.png" height="80%" width="100%"/>
- <b>Select the "Active Directory Domain Services," "Add Features," hit "Next" for the rest of the tabs.<br>
<br/>
<img src="https://i.imgur.com/dpV1Xby.png" height="80%" width="100%"/>
- <b>Lastly Install, the installation will take several minutes to complete.<br>
<br/>

<h2>Creating the Domain</h2>
<img src="https://i.imgur.com/smZch5Z.png" height="80%" width="100%"/>
- <b>Click on the flag then click on "Promote this server to a domain controller"<br>
<br/>
<img src="https://i.imgur.com/rvBPsod.png" height="80%" width="100%"/>
- <b>Select "Add a new forest" and create a Root domain name (the name chosen for the lab is "mydomain.com")<br>
<br/>
<img src="https://i.imgur.com/6ufbTde.png" height="80%" width="100%"/>
- <b>Create a password ("Password1" was used for this lab step)<br>
<br/>
<img src="https://i.imgur.com/R9pV3bp.png" height="80%" width="100%"/>
- <b>(RED BOX) Hit "Next" for the rest of the tabs and "Install." This will take several minutes and cause your Virtual Box to restart.<br>
<br/>

<h2>Creating a Domain Administrator Account</h2>
<img src="https://i.imgur.com/whZg1kW.png" height="80%" width="100%"/>
- <b>After restarting, we notice a change in account name. Login with the password created (Password1).<br>
<br/>
<img src="https://i.imgur.com/bToCY4g.png" height="80%" width="100%"/>
- <b>Navigate through the start menu to "Active Directory Users and Computers"<br>
<br/>
<img src="https://i.imgur.com/ZMLzSBO.png" height="80%" width="100%"/>
- <b>Our newly created domain "mydomain.com" appears, right click it to create an "Organizational Unit (OU)" to put our admin account in.<br>
  <br/>
<img src="https://i.imgur.com/Inq4b9I.png" height="80%" width="100%"/>
- <b>Name it off your preference (used "_ADMINS")<br>
  <br/>
<img src="https://i.imgur.com/SHkRbcT.png" height="80%" width="100%"/>
- <b>Now right click on the new OU ("_ADMINS") to create a new user a.k.a. the Domain Admin Account <br>
  <br/>
<img src="https://i.imgur.com/C3moeeC.png" height="80%" width="100%"/>
- <b>Type your full name with the user login starting with an "a-" (common form of admin accounts in companies starting with a) followed by the first initial of the name with lastly followed with the last name.<br>
  <br/>
<img src="https://i.imgur.com/D88Dr2o.png" height="80%" width="100%"/>
- <b>Create a password ("Password1") and make sure to check "Password never expires"<br>
  <br/>
<img src="https://i.imgur.com/Q8ketj1.png" height="80%" width="100%"/>
- <b>After creating the new user, it is illustrated in "_ADMINS" (OU).<br>
- <b>Right click to go the account's "Properties"<br>
<br/>
<img src="https://i.imgur.com/WLBYPAK.png" height="80%" width="100%"/>
- <b>To officially make it a Domain Admin Account, (RED BOXES) Member Of -> Add... -> "Domain Admins" -> Check Names<br>
- <b>Next, sign out of the "MYDOMAIN\Administrator" account using the Start Menu.
  <br/>
<img src="https://i.imgur.com/oLhqEfK.png" height="80%" width="100%"/>
- <b>Sign in using "Other user" and enter the Domain Admin Account user (a-jluong) and password (Password1) that was created.<br>
- <b>Note below that it now says "Sign in to: MYDOMAIN"<br>
<br/>

<h2>Installing RAS/NAT</h2>
<img src="https://i.imgur.com/duJzjf5.png" height="80%" width="100%"/>
<img src="https://i.imgur.com/KypVEsQ.png" height="80%" width="100%"/>
- <b>Now we're adding another role, similar to when installing AD DS but now we are checking the "Remote Access" box <br>
  <br/>
<img src="https://i.imgur.com/0dM8w7b.png" height="80%" width="100%"/>
- <b>And select "Routing" for the role services and hit "Add Features"<br>
  <br/>
<img src="https://i.imgur.com/kOaGT1K.png" height="80%" width="100%"/>
- <b>Then Install the role service which will take several minutes.<br>
  <br/>
<img src="https://i.imgur.com/lTx8ujM.png" height="80%" width="100%"/>
- <b>Tools -> Routing and Remote Access<br>
  <br/>
<img src="https://i.imgur.com/XUMxHpv.png" height="80%" width="100%"/>
- <b>Right click DOMAINCONTROLLER -> Configure and Enable Routing and Remote Access -> Next<br>
  <br/>
<img src="https://i.imgur.com/rBuluD7.png" height="80%" width="100%"/>
- <b>Select "Network address translation (NAT)" as the purpose is as described in the highlighted Red box.<br>
  <br/>
<img src="https://i.imgur.com/x2YtYxN.png" height="80%" width="100%"/>
- <b>Select the external network (Xx_Internet_xX) that was renamed by identifying it's IP address.<br>
- <b>Then hit Next and then Finish to complete this step.<br>
- <b>Note if you don't see it the first time, close out the window and retry again.<br>
  <br/>
<img src="https://i.imgur.com/2Pz3PV3.png" height="80%" width="100%"/>
- <b>If followed properly, it should look like this where the DOMAINCONTROLLER is now green and have successfully configured RAS/NAT.<br>
<br/>

<h2>Setting up the DHCP Server</h2>
<img src="https://i.imgur.com/duJzjf5.png" height="80%" width="100%"/>
<img src="https://i.imgur.com/LaFyAR4.png" height="80%" width="100%"/>
- <b>Repeat the same steps but now we are going to select the box "DHCP Server" and "Add Features"<br>
- <b>Continue through the tabs similar to the previous steps to Install which will take several minutes.<br>
  <br/>
<img src="https://i.imgur.com/zqNAOko.png" height="80%" width="100%"/>
<img src="https://i.imgur.com/miaN8Er.png" height="80%" width="100%"/>
- <b>After going through "Tools" -> "DHCP," right click "IPv4" -> "New Scope"<br>
- <b>A pop up window is going to appear and thus hit "Next"<br>
  <br/>
<img src="https://i.imgur.com/M1Aw9xp.png" height="80%" width="100%"/>
- <b>Enter any Scope Name, for this lab I entered the Scope Range (172.16.0.100-200), then hit Next <br>
  <br/>
<img src="https://i.imgur.com/lXCBQUd.png" height="80%" width="100%"/>
- <b>The "Start IP address:" is the beginning range (172.16.100) while "End IP Address:" is the end range (172.16.0.200).<br>
- <b>The (CIDR) "Length" will be set to (/)24 which automatically inputs the mask as 255.255.255.0 <br>
- <b>After proceeding to "Next" it will ask to add any Exclusions or Delays, skip it and proceed to "Next"<br>
  <br/>
<img src="https://i.imgur.com/TDFpysU.png" height="80%" width="100%"/>
- <b>"Lease Duration" is how long a computer can hold an IP Address before it becomes refreshed for another user to use. I inputed 8 days, but it ranges depending on circumstanes whether it be at a cafe, school, library, or company for example.<br>
  <br/>
<img src="https://i.imgur.com/rB4KBIR.png" height="80%" width="100%"/>
- <b>Select the "Yes, I want to configure these options now" because we want the client to use specific servers/gateways to connect to the internet.<br>
  <br/>
<img src="https://i.imgur.com/CK22avW.png" height="80%" width="100%"/>
- <b>Enter the IP Address of the Domain Controlller which serves as both the default gateway and DNS. Afterwards, hit "Add"<br>
- <b>After adding, proceed with all "Next" and then "Finish"<br>
  <br/>
<img src="https://i.imgur.com/k8GaYn6.png" height="80%" width="100%"/>
- <b>Right click domaincontrollerpc.mydomain.com to "Authorize" and then "Refresh" as well in the drop down menu.<br>
  <br/>
<img src="https://i.imgur.com/4glHete.png" height="80%" width="100%"/>
- <b>After refreshing, IPv4, IPv6, Address Lease, and the Scope are now setup thus the DNS server running for the Domain Controller. <br>
<br/>

<h2>Downloading the Script and Generated Users</h2>
<img src="https://i.imgur.com/FOzNaHh.png" height="80%" width="100%"/>
<img src="https://i.imgur.com/zaBccFq.png" height="80%" width="100%"/>
- <b>Before using the internet and downloading the script, turn off the "Internet Explorer Enhanced Security Configuration" to disable pop up windows when opening internet explorer.<br>
  <br/>
<img src="https://i.imgur.com/1IHnd98.png" height="80%" width="100%"/>
<img src="https://i.imgur.com/Wnyko3r.png" height="80%" width="100%"/>
- <b>Download the files from this link provided by Josh Madakor, 
  "[https://github.com/joshmadakor1/AD_PS]"<br>
- <b>"Save As" into your Desktop once downloaded.<br>
  <br/>
<img src="https://i.imgur.com/XQU0Gzq.png" height="80%" width="100%"/>
- <b>Open the "Notepad" file with the generated names, remove the first name on the list, and enter your name that will be made as a user and as an admin account.<br>
<br/>

<h2>Running the Script in Windows Powershell ISE</h2>
<img src="https://i.imgur.com/vCRIIXU.png" height="80%" width="100%"/>
- <b>Open Windows Powershell ISE in administrator mode<br>
  <br/>
<img src="https://i.imgur.com/CHwKD61.png" height="80%" width="100%"/>
- <b>Open the downloaded script "1_CREATE_USERS"<br>
  <br/>
<img src="https://i.imgur.com/kWUjmll.png" height="80%" width="100%"/>
- <b>(RED BOX) When running the script, you'll receive an error because the file is not "digitally signed."<br>
- <b>(ORANGE BOX) To bypass, type "Set-ExecutionPolicy Unrestricted", press enter, and click "Yes to All"<br>
  <br/>
<img src="https://i.imgur.com/Iywu2AY.png" height="80%" width="100%"/>
<img src="https://i.imgur.com/aQVyPqu.png" height="80%" width="100%"/>
- <b>(RED BOX) Before running the script, change to the directory first by typing "cd C:\users\a-luong\Desktop\AD_PS-master"<br>
- <b>(ORANGE BOX) Type "ls" to list the files present.<br>
  <br/>
<img src="https://i.imgur.com/tro3LtT.png" height="80%" width="100%"/>
- <b>Now you can run the script which creates and lists the usernames in a black background and cyan font.<br>
  <br/>
<img src="https://i.imgur.com/pRrflWG.png" height="80%" width="100%"/>
- <b>(RED BOX) To view the list of users or if you wanted to find a specific viewer, go to "Active Directory Users and Computers" in the start menu and navigate to "mydomain.com"<br>
- <b>(ORANGE BOX)From there, you'll see a "USERS" tab present now, double click and type any specific first name, last name, or first and last name. Click "Find New" and from there it will pop up in the results if the name exists within the list.<br>
<br/>

<h2>Setting up Windows 10 ISO Virtual Machine</h2>
<img src="https://i.imgur.com/EOV0iDq.png" height="80%" width="100%"/>
- <b>Click "New", enter any name for the VM, and set the version to "Windows 10 (64-bit)<br>
  <br/>
<img src="https://i.imgur.com/Zydaiq0.png" height="80%" width="100%"/>
- <b>Set the RAM (4096 MB) and CPU (4) to what your PC can handle comfortably<br>
  <br/>
<img src="https://i.imgur.com/CS4BB28.png" height="80%" width="100%"/>
- <b>Go to the settings -> Advanced tab -> and changed both options to "Bidirectional"<br>
  <br/>
<img src="https://i.imgur.com/mcppxCn.png" height="80%" width="100%"/>
- <b>In the network tab, change Adapter 1 to an "Internal Network" since it's obtaining its own DHCP address from the domain controller<br>
- <b>This way of connecting to the other Internal Network is similar as how school systems or companies operate.<br>
  <br/>
<img src="https://i.imgur.com/xDccKdo.png" height="80%" width="100%"/>
- <b>Double click the new created VM and select "Other" for the DVD<br>
  <br/>
<img src="https://i.imgur.com/uXsHAqg.png" height="80%" width="100%"/>
- <b>Attach the WIndows 10 ISO file to the new VM and continue.<br>
  <br/>
<img src="https://i.imgur.com/nxX2Df9.png" height="80%" width="100%"/>
- <b>Choose your language preference.<br>
  <br/>
<img src="https://i.imgur.com/PpzPpF7.png" height="80%" width="100%"/>
- <b>Select "I Don't have a product key"<br>
  <br/>
<img src="https://i.imgur.com/CNkyklw.png" height="80%" width="100%"/>
- <b>Select "Custom: Install Windows only (Advanced)"<br>
  <br/>
<img src="https://i.imgur.com/vqxaXNA.png" height="80%" width="100%"/>
- <b>Select "I don't have internet"<br>
  <br/>
<img src="https://i.imgur.com/ffklCuq.png" height="80%" width="100%"/>
- <b>Select "Continue with limited setup"<br>
  <br/>
<img src="https://i.imgur.com/EksuPSk.png" height="80%" width="100%"/>
- <b>Enter any name for the user.<br>
  <br/>
<img src="https://i.imgur.com/VlJoOsq.png" height="80%" width="100%"/>
- <b>Select "No" for all, (optional)<br>
  <br/>
<img src="https://i.imgur.com/AoFme25.png" height="80%" width="100%"/>
- <b>To ensure that your new virtual machine is connected to the domain controller, open the "Command Prompt" in the Windows Start Menu, and enter (RED BOX) "ipconfig" which will illustrate the IPv4 Address and the (ORANGE BOX) Default Gateway address.<br>
- <b>In addition, pinging any site such as (RED BOX) "www.google.com" results in an (ORANGE BOX) address output which means that the this VM is connected to the other internal network, that's connected to the domain controller, that's connected to the external network, and thus is connected to the internet.<br>
- <b>Lastly when entering (RED BOX) "hostname", it outputs the name given to the PC. Companies would want to rename in case their's a personal laptop under the company which is assigned to a specific user.<br>
  <br/>
<img src="https://i.imgur.com/HfTjkak.png" height="80%" width="100%"/>
- <b>To rename the PC, go to the about page in your settings and select "Rename this PC (advanced)" <br>
  <br/>
<img src="https://i.imgur.com/0t9SJnv.png" height="80%" width="100%"/>
- <b>"Change" -> Rename as desired (CLIENT1) -> "Domain (mydomain.com)" -> Enter username and password for the VM to confirm changes. Then restart the client to confirm changes.<br>
  <br/>
<img src="https://i.imgur.com/uqEsjZz.png" height="80%" width="100%"/>
- <b>To also view the changes, go to the "DomainController" VM and view the DHCP -> IPv4 -> Scope -> Address Lease<br>
- <b>There you will notice the name of the PC has changed to "Client1" and it's present in the DHCP since the CLIENT1's VM requested a DHCP address.<br>
  <br/>
<img src="https://i.imgur.com/MGOZEYt.png" height="80%" width="100%"/>
<img src="https://i.imgur.com/9XWmE1O.png" height="80%" width="100%"/>
- <b>Another way of viewing is going to "Active Directory Users and Computers" -> "Computers"<br>
- <b>"CLIENT1" is the computer that's connected to the domain controller in which any username that was created from the previous script that was ran can be used to log into that specific PC.<br>

