<p align="center">
  
![network](https://github.com/user-attachments/assets/99258344-ef0d-4a61-b1f5-0bbb262191a5)

</p>

<h1>Monitoring Network Traffic</h1>
<h2>Description</h2>
This project consists of creating two virtual machines in Azure and monitoring traffic on the network using Wireshark<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure
- Virtual Machines
- Remote Desktop Connection
- Wireshark
- Powershell
- Various Network Protocols (ICMP, SSH, DHCP, DNS)

<h2>Operating Systems Used </h2>

- Windows 10 Pro</b> (22H2)
- Ubuntu 24.04</b>

<h2>Project Walk-Through:</h2>

<h3>Step 1.</h3>

![1  go to resource groups](https://github.com/user-attachments/assets/8ff5169b-4f14-460c-a58f-bcc2708a9f2c)

<p>Go to resource groups in Azure</p>

<h3>Step 2.</h3>

![2  click create](https://github.com/user-attachments/assets/ece20628-9593-4a54-a4ed-2643d7511658)

<p>Click Create</p>

<h3>Step 3.</h3>

![3  name resource group](https://github.com/user-attachments/assets/ac5bfa96-cfd3-4ce0-b28c-0bd500860c22)

<p>Name the resource group, select the region, then click Review + create</p>

<h3>Step 4.</h3>

![4  create the resource group](https://github.com/user-attachments/assets/6e5cb6dc-87ad-41c2-995d-e3765a19c838)

<p>Click Create</p>

<h3>Step 5.</h3>

![5  resource group created](https://github.com/user-attachments/assets/1e2bc588-73e1-4064-91a4-9063f0fa4d98)

<p>The resource group has now been created</p>

<h3>Step 6.</h3>

![6  search virtual machines](https://github.com/user-attachments/assets/33c2fc30-26a2-426d-9b27-c4c67f2269d8)

<p>Now search for Virtual Machines in Azure</p>

<h3>Step 7.</h3>

![7  click create vm](https://github.com/user-attachments/assets/f4464a53-f614-40b0-b07a-fddebeb5408c)

<p>Click Create Azure Virtual Machine</p>

<h3>Step 8.</h3>

![8  setup vm settings](https://github.com/user-attachments/assets/57e32226-69ea-4fac-9bfc-693b54f3e48b)

<p>Select the resource group we created, name the vm, select the region, select Windows 10 Pro version 22H2 for the image, and pick a size of 2vcpus 8 GiB memory</p>

<h3>Step 9.</h3>

![9  vm user   pass](https://github.com/user-attachments/assets/ac1c2983-cd72-4463-8358-59ef69067243)

<p>Create a user and password for this vm, check the box, then click Next : Disks ></p>

<h3>Step 10.</h3>

![10  next](https://github.com/user-attachments/assets/3179ed9e-0a04-44d8-827f-455d8b80b065)

<p>Click Next : Networking ></p>

<h3>Step 11.</h3>

![11  create vnet](https://github.com/user-attachments/assets/18a2cd46-84bf-4282-94e8-c14b505398ae)

<p>Click create new virtual network, name the virtual network, then click OK</p>

<h3>Step 12.</h3>

![12  review   create](https://github.com/user-attachments/assets/601b4f3b-21be-405e-a4f2-47274c87a079)

<p>Click Review + create</p>

<h3>Step 13.</h3>

![13  click create](https://github.com/user-attachments/assets/a3982295-46df-4134-8e53-3ea8bde4aaae)

<p>Click Create</p>

<h3>Step 14.</h3>

![14  deployment complete](https://github.com/user-attachments/assets/aba2d49a-f645-47e7-a7c4-8b5eefa361d1)

<p>The first virtual machine has been created</p>

<h3>Step 15.</h3>

![15  search vm's](https://github.com/user-attachments/assets/3523a5d6-5ec8-4857-ac69-f5f6c55f2d2b)

<p>Search for Virtual Machines in Azure again</p>

<h3>Step 16.</h3>

![16  click create vm](https://github.com/user-attachments/assets/12214033-0716-4b32-8563-c5ee218343d7)

<p>Click Create Azure Virtual Machine</p>

<h3>Step 17.</h3>

![17  vm details](https://github.com/user-attachments/assets/8a119177-f41f-4f48-ba6b-8fe609a286d5)

<p>Select the resource group we created, name the vm, select the region, select Ubuntu Server version 22.04 for the image, and pick a size of 2vcpus 8 GiB memory</p>

<h3>Step 18.</h3>

![18  vm user   pass linux](https://github.com/user-attachments/assets/39341ada-33f3-4234-9b42-c5463cd122f5)

<p>Select password option, create a user and password for this vm, then click Next : Disks ></p>

<h3>Step 19.</h3>

![19  next networking](https://github.com/user-attachments/assets/9c24c651-7ef6-44f8-a4b1-6aa1e8c26adb)

<p>Click Next : Networking ></p>

<h3>Step 20.</h3>

![20  vnet name review](https://github.com/user-attachments/assets/b2205490-34ab-49de-8a96-24e73a2a6a7b)

<p>Select the virtual network we created, then click Review + create</p>

<h3>Step 21.</h3>

![21  create](https://github.com/user-attachments/assets/91129891-912d-49f9-9830-15a8b63f21d2)

<p>Click Create</p>

<h3>Step 22.</h3>

![22  linux vm created](https://github.com/user-attachments/assets/eaa1cb2b-1d46-4307-afe6-90569f1320ab)

<p>The second virtual machine has been deployed</p>

<h3>Step 23.</h3>

![23  view vms](https://github.com/user-attachments/assets/e96d8082-3656-4393-9789-15041510b314)

<p>Both the Linux and Windows vms are now deployed and running</p>

<h3>Step 24.</h3>

![24  verify vnet](https://github.com/user-attachments/assets/92e401f5-f0ea-444c-84fd-39362f0a52e1)

<p>Verify the Linux and Windows vm are on the same virtual network</p>

<h3>Step 25.</h3>

![25  verify vnet](https://github.com/user-attachments/assets/a44b8468-616b-4413-bfe5-ca4eaf8e1edf)

<p>Verify the Linux and Windows vm are on the same virtual network</p>

<h3>Step 26.</h3>

![1  select windows vm](https://github.com/user-attachments/assets/a29733cb-129d-4f1c-9b59-c27d907745fb)

<p>Select the Windows VM</p>

<h3>Step 27.</h3>

![2  copy public ip](https://github.com/user-attachments/assets/d22e1e66-91bc-4a4a-a61b-005db86f3d92)

<p>Get the public IP address</p>

<h3>Step 28.</h3>

![3  open remote desktop](https://github.com/user-attachments/assets/e4724824-1a3a-4a9f-ba2a-240e5609925f)

<p>Open Remote Desktop Connection and enter the public IP of the Windows vm, then click Connect</p>

<h3>Step 29.</h3>

![4  enter credentials](https://github.com/user-attachments/assets/7b8774bd-b843-4a4d-838f-4e9e29784978)

<p>Enter the username and password for the Windows VM, then click OK</p>

<h3>Step 30.</h3>

![5  inside vm](https://github.com/user-attachments/assets/800d2bf3-a8f9-4b3c-b94c-a1623448934c)

<p>Inside the Windows VM, open Microsoft Edge</p>

<h3>Step 31.</h3>

![6  go to wireshark](https://github.com/user-attachments/assets/e4ca5282-2ba5-4290-acfa-471ece331669)

<p>Go to https://www.wireshark.org and click Download</p>

<h3>Step 32.</h3>

![7  download wireshark](https://github.com/user-attachments/assets/d2387185-473a-431f-b0b5-f69d31d71fcd)

<p>Click Windows x64 Installer and start the download</p>

<h3>Step 33.</h3>

![8  go through setup and install](https://github.com/user-attachments/assets/3ef1fa6f-c55b-415e-a66f-a6f949564ac0)

<p>Open the downloaded file and go through the Wireshark setup</p>

<h3>Step 34.</h3>

![9  installing](https://github.com/user-attachments/assets/3b3c775c-81b7-4907-a239-eb6be8a082e3)

<p>Install Wireshark</p>

<h3>Step 35.</h3>

![10  find newly installed wireshark](https://github.com/user-attachments/assets/8e6351c4-93f9-47f1-9627-8fede2fdf5fb)

<p>Search for Wireshark in the Windows search bar and open it</p>

<h3>Step 36.</h3>

![11  select ethernet](https://github.com/user-attachments/assets/a788992d-5004-4a0c-a2d6-cabb494c61d9)

<p>Select Ethernet</p>

<h3>Step 37.</h3>

![12  network traffic](https://github.com/user-attachments/assets/cff97648-0b0e-40cb-80e1-d624a4ffe053)

<p>Now you should see all of the network traffic within Wireshark</p>

<h3>Step 38.</h3>

![13  filter icmp only](https://github.com/user-attachments/assets/cd051032-7ee2-40e3-9781-74a5b8308ff9)

<p>Now filter for ICMP traffic by entering "icmp" in the bar at the top</p>

<h3>Step 39.</h3>

![15  open powershell](https://github.com/user-attachments/assets/1a7e4596-edc8-4c31-8734-b1e69a5b88a3)

<p>Search for Windows Powershell in the Windows search bar and open it</p>

<h3>Step 40.</h3>

![16  type ping](https://github.com/user-attachments/assets/174ba0a3-c759-49fe-ac60-155c58c1af87)

<p>Issue a ping command by typing ping 10.0.0.5, this will ping the Linux virtual machine's private IP address</p>

<h3>Step 41.</h3>

![17  ping results](https://github.com/user-attachments/assets/53e55c89-71e5-427a-a9ac-e41ff62ada39)

<p>This should give us a response from the Linux VM and we can now see the ICMP traffic within Wireshark</p>

<h3>Step 42.</h3>

![18  nonstop ping](https://github.com/user-attachments/assets/0138a876-e084-4b1b-854f-c64670db7397)

<p>Issue a nonstop ping command to the Linux VM by entering "ping 10.0.0.5 -t" into Powershell. Now restart the capture within Wireshark by clicking the fin icon.</p>

<h3>Step 43.</h3>

![19  ping results](https://github.com/user-attachments/assets/2bfeac40-3896-4c3f-8a6c-722fb1ce7bab)

<p>Now it will continously ping the Linux VM and we can see the ICMP traffic within Wireshark</p>

<h3>Step 44.</h3>

![20  nsg](https://github.com/user-attachments/assets/13a752ac-0e6e-463e-b19a-9a28d0a2934e)

<p>Now go back to azure and go to the Network Security Group for the Linux VM</p>

<h3>Step 45.</h3>

![21  add inbound rule](https://github.com/user-attachments/assets/8a5ebfed-473c-4ee9-92a6-eef18552c32b)

<p>Go to Settings, Inbound security rules, and click Add</p>

<h3>Step 46.</h3>

![22  rule settings](https://github.com/user-attachments/assets/346657e8-a85e-477c-bc21-095bd36fbeed)

<p>Put the port ranges as "*", select ICMPv4, select Deny, put the priority as 293, then click Add</p>

<h3>Step 47.</h3>

![23  rule added](https://github.com/user-attachments/assets/0f0315d7-8506-449f-967c-113ac2e0e149)

<p>The new security rule has been added. This will deny any inbound ICMP traffic to the Linux VM.</p>

<h3>Step 48.</h3>

![24  rule results](https://github.com/user-attachments/assets/90864802-2c4d-4e87-99fb-01698442a859)

<p>Now the ping requests in Powershell are timing out and there is only request traffic in Wireshark. This is the result of the new security rule</p>

<h3>Step 49.</h3>

![25  deleting rule](https://github.com/user-attachments/assets/4836745f-418e-4b50-9e9a-d504f316bbae)

<p>Now go back to Azure in the Network Security Group for the Linux VM and delete the rule we created.</p>

<h3>Step 50.</h3>

![26  ping results after deletion](https://github.com/user-attachments/assets/cdc81174-e007-4805-9d1d-d1a22c1753c3)

<p>As you can see we are now getting replies again from the Linux VM after deleting the rule. This is evident in Powershell and Wireshark </p>

<h3>Step 51.</h3>

![27  stop ping   capture](https://github.com/user-attachments/assets/658a3eed-a073-4c74-a5e0-dd83fc0cf2e2)

<p>Press CTRL + C to stop the nonstop ping command in Powershell and click the stop button in Wireshark to stop the capture</p>

<h3>Step 52.</h3>

![28  add ssh filter](https://github.com/user-attachments/assets/f32c7d46-4ddc-4a52-8375-bb3c68edb348)

<p>Now add an SSH filter inside of Wireshark by entering "ssh" in the top bar</p>

<h3>Step 53.</h3>

![29  get private ip linux](https://github.com/user-attachments/assets/a43e3c4d-6c64-4a3f-8bd9-e0237546cee5)

<p>Grab the private IP of the Linux VM</p>

<h3>Step 54.</h3>

![30  ssh ps command](https://github.com/user-attachments/assets/961bfef4-925a-4cfe-bee9-d359d37ed0dc)

<p>Issue an ssh command inside of Powershell by typing "ssh username@10.0.0.5" using the username and private IP of the Linux VM</p>

<h3>Step 55.</h3>

![31  ssh into linux](https://github.com/user-attachments/assets/3f0a220c-643b-4045-8a2d-a2a3526bd4e1)

<p>Enter the password for the Linux VM into Powershell, the SSH traffic should now appear within Wireshark</p>

<h3>Step 56.</h3>

![32  ssh success](https://github.com/user-attachments/assets/5c72f0e8-7e54-4453-a008-b1eaa7c0038b)

<p>The SSH into the Linux VM should have succeeded. You can check by using the commands shown in the screenshot.</p>

<h3>Step 57.</h3>

![33  ssh closed](https://github.com/user-attachments/assets/d69661f3-dfb7-497c-b060-16d31ce6e8e6)

<p>Now close the SSH by typing the "exit" command</p>

<h3>Step 58.</h3>

![34  making dhcp script](https://github.com/user-attachments/assets/41ff6799-917e-4518-b11d-553bc8b75ae8)

<p>Open notepad and make 2 lines of text with ipconfig /release and ipconfig /renew</p>

<h3>Step 59.</h3>

![35  saving script](https://github.com/user-attachments/assets/02b8ec6f-2bed-41c8-b89d-c6c3a39e8e15)

<p>Name the file dhcp.bat, select All Files as the type, annd click Save</p>

<h3>Step 60.</h3>

![36  saved](https://github.com/user-attachments/assets/1c84297d-5ba1-436c-add3-8a88acc6c7f0)

<p>The script/batch file has now been created</p>

<h3>Step 61.</h3>

![37  running dhcp script](https://github.com/user-attachments/assets/d4af0c29-8e2f-4304-b2fb-13476e92c53a)

<p>Run the script by typing "./dhcp.bat" into powershell and filter for "udp.port == 67 || udp.port == 68" in Wireshark</p>

<h3>Step 62.</h3>

![38  dhcp traffic results](https://github.com/user-attachments/assets/73006544-e9d8-4459-8a84-a8fc97d82e6f)

<p>This script will release our VM's IP address and request a new one from the DHCP server. We will likely get the same IP as we had previous. The DHCP traffic can now be seen inside Wireshark.</p>

<h3>Step 63.</h3>

![39  dns filter](https://github.com/user-attachments/assets/d8413da2-b189-4edf-bfd3-1e85f9c23da2)

<p>Filter for DNS traffic by entering "dns" in the top bar of Wireshark, Then issue the command nslookup in Powershell by typing "nslookup disney.com"</p>

<h3>Step 64.</h3>

![40  dns results](https://github.com/user-attachments/assets/199dcd7b-8e00-48bb-b3b0-66d345eb1e20)

<p>The DNS server should now reveal the IP address associated with disney.com in Powershell and you can see the DNS traffic within Wireshark.</p>

<h3>Step 65.</h3>

![41  rdp filter   results](https://github.com/user-attachments/assets/7d2c6834-ccb9-4666-81be-cb0b24918bb9)

<p>Now filter for Remote Desktop Protocol by entering "tcp.port == 3389" in the top bar of Wireshark. This should now show the network traffic for RDP because we are inside of a Windows virtual machine using Remote Desktop Connection which is showing a constant livestream of what is happening.</p>

<h2>Monitoring Network Traffic Complete!</h2>

<p>In this project, we have successfully created two virtual machines, one running Linux Server, and one running Windows 10. We installed Wireshark and analyzed network traffic of various protocols such as ICMP, SSH, DHCP, and DNS by issuing commands inside Powershell.</p>


