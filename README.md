<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Computer)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)


<h2>High-Level Deployment and Configuration Steps</h2>

- Step 1: Install Active Directory

- Step 2: Create a Domain User within the Domain 

- Step 3: Join Client-1 to your domain (mydomain.com)

- Step 4: Setup Remote Desktop for non-administrative users on Client-1

- Step 5: Create additional users and attempt to log into client-1 with one of the users
<p>

<h2>Deployment and Configuration Steps</h2>

<h3> Step 1: Install Active Directory</h3>

- Login to DC-1 and install Active Directory Domain Services
  
- Promote as a DC: Setup a new forest as mydomain.com (can be anything, just
remember what it is)

- Restart and then log back into DC-1 as user: mydomain.com\labuser

<br />

<p>
<img width="1841" height="587" alt="Screenshot 2026-01-07 175822" src="https://github.com/user-attachments/assets/57450151-8522-46d8-b976-6667d841a167" />
</p>

<p>
<img width="448" height="270" alt="Screenshot 2026-01-07 175859" src="https://github.com/user-attachments/assets/e5edfbfe-7cab-4501-9fa5-186c070d7303" />
</p>

<p>
<img width="665" height="680" alt="Screenshot 2026-01-07 180208" src="https://github.com/user-attachments/assets/8810c444-ea60-41fa-985e-8349b7d07509" />
</p>

<p>
<img width="1255" height="769" alt="Screenshot 2026-01-07 180249" src="https://github.com/user-attachments/assets/a68769e9-30f0-46ff-ad84-80300f35b171" />
</p>

<p>
<img width="807" height="575" alt="Screenshot 2026-01-07 180343" src="https://github.com/user-attachments/assets/bd09a2af-c97d-4280-bb44-1f5725214366" />
</p>

<p>
<img width="825" height="575" alt="Screenshot 2026-01-07 180350" src="https://github.com/user-attachments/assets/c191c466-4b8e-43b8-8b77-b16cee06c93e" />
</p>

<p>
<img width="829" height="591" alt="Screenshot 2026-01-07 180405" src="https://github.com/user-attachments/assets/df222072-7fd5-4ba1-882e-07e9b46e2564" />
</p>

<p>
<img width="825" height="575" alt="Screenshot 2026-01-07 180448" src="https://github.com/user-attachments/assets/6209c4b3-ae35-4c8f-8ada-3cf1f8a37684" />
</p>

<p>
<img width="808" height="571" alt="Screenshot 2026-01-07 180501" src="https://github.com/user-attachments/assets/8f52d596-9881-4fad-a38e-6e8b71b6fe0c" />
</p>

<p>
<img width="829" height="581" alt="Screenshot 2026-01-07 180508" src="https://github.com/user-attachments/assets/c9bb5793-4a4e-4e20-aadf-cb48f3acf1a3" />

</p>

<p>
<img width="1318" height="571" alt="Screenshot 2026-01-07 180542" src="https://github.com/user-attachments/assets/91d058cf-3609-40c4-a951-3545f680a03a" />
</p>

<p>
<img width="1041" height="452" alt="Screenshot 2026-01-07 180758" src="https://github.com/user-attachments/assets/bed4209e-7334-4a76-a4e4-807a98b5031f" />

</p>

<p>
<img width="787" height="565" alt="Screenshot 2026-01-07 180837" src="https://github.com/user-attachments/assets/b2fcfcf8-4476-4eb6-a6c5-e3e3e6ebf16f" />

</p>

<p>
<img width="786" height="566" alt="Screenshot 2026-01-07 180900" src="https://github.com/user-attachments/assets/ee6411b0-ae7f-4232-adb0-ba231ea07ef9" />

</p>

<p>
<img width="781" height="575" alt="Screenshot 2026-01-07 180950" src="https://github.com/user-attachments/assets/9c3db561-af29-49ef-8a50-85957a880829" />

</p>

<p>
<img width="793" height="577" alt="Screenshot 2026-01-07 180958" src="https://github.com/user-attachments/assets/9bffab60-761a-4d2e-a35c-72cab20f4b05" />

</p>

<p>
<img width="780" height="574" alt="Screenshot 2026-01-07 181047" src="https://github.com/user-attachments/assets/c056daab-c6b9-4628-8963-753f04e94565" />

</p>

<p>
<img width="790" height="580" alt="Screenshot 2026-01-07 181054" src="https://github.com/user-attachments/assets/b9071b8c-df5a-4282-aae5-5b341bcf15ef" />

</p>

<p>
<img width="778" height="573" alt="Screenshot 2026-01-07 181117" src="https://github.com/user-attachments/assets/d4bb29de-5d5c-4b72-a698-6017ed799c06" />

</p>

<p>
<img width="785" height="584" alt="Screenshot 2026-01-07 181145" src="https://github.com/user-attachments/assets/b9224b9c-ff1c-4436-911e-5a1fa06845e1" />

</p>

<p>
<img width="1443" height="821" alt="Screenshot 2026-01-07 181413" src="https://github.com/user-attachments/assets/be45f443-a73d-4740-9c2f-f9ca0ffcafb8" />

</p>

<p>
<img width="422" height="247" alt="Screenshot 2026-01-07 181444" src="https://github.com/user-attachments/assets/61a1900d-ce77-4b31-aad9-e52dc6a7fe21" />

</p>

<p>
<img width="467" height="571" alt="Screenshot 2026-01-07 182120" src="https://github.com/user-attachments/assets/e7498052-5e3a-4bbe-a3b8-8773ecf5c2f0" />

</p>
<br />

<h3> Step 2: Create a Domain Admin user within the domain</h3>

- In Active Directory Users and Computers (ADUC), create an Organizational Unit
(OU) called “_EMPLOYEES”

- Create a new OU named “_ADMINS”
  
- Create a new employee named “Jane Doe” (same password) with the username
of “jane_admin” / Password1

- Add jane_admin to the “Domain Admins” Security Group
  
- Log out / close the connection to DC-1 and log back in as
“mydomain.com\jane_admin”

- Use jane_admin as your admin account from now on
</p>
<br />

<p>
<img width="666" height="685" alt="Screenshot 2026-01-07 182503" src="https://github.com/user-attachments/assets/9a582f4e-2313-45c2-8b1b-1d8e07359a04" />

</p>

<p>
<img width="663" height="684" alt="Screenshot 2026-01-07 182526" src="https://github.com/user-attachments/assets/ebfa9938-6854-4c3c-9b97-fc1857c6b26c" />

</p>

<p>
<img width="689" height="562" alt="Screenshot 2026-01-07 182817" src="https://github.com/user-attachments/assets/594f79e8-ceee-4059-8105-91b50e149649" />

</p>

<p>
<img width="456" height="365" alt="Screenshot 2026-01-07 182940" src="https://github.com/user-attachments/assets/2e48a397-2379-4723-9086-ed4efff44a94" />

</p>

<p>
<img width="622" height="479" alt="Screenshot 2026-01-07 183006" src="https://github.com/user-attachments/assets/30f7762d-b1bc-433f-8ae3-237efe2aa97c" />

</p>

<p>
<img width="459" height="363" alt="Screenshot 2026-01-07 183030" src="https://github.com/user-attachments/assets/3bfca9ec-fd58-4efd-96ab-5eb7b358ac47" />

</p>

<p>
<img width="564" height="514" alt="Screenshot 2026-01-07 183202" src="https://github.com/user-attachments/assets/c770a213-4863-45b5-9870-4b39fe254e74" />

</p>

<p>
<img width="458" height="364" alt="Screenshot 2026-01-07 183246" src="https://github.com/user-attachments/assets/7bab7665-2bff-47a0-a293-390250d7dd6d" />

</p>

<p>
<img width="452" height="366" alt="Screenshot 2026-01-07 183340" src="https://github.com/user-attachments/assets/948eaafc-efa9-4eaf-a1be-4d7dbd689113" />

</p>

<p>
<img width="465" height="362" alt="Screenshot 2026-01-07 183349" src="https://github.com/user-attachments/assets/ed976f43-fe74-47f4-ad2f-5e429eb07a4c" />

</p>

<p>
<img width="659" height="433" alt="Screenshot 2026-01-07 183448" src="https://github.com/user-attachments/assets/97b0f7da-01b8-4c6b-8150-da3092a1fcf3" />

</p>

<p>
<img width="452" height="579" alt="Screenshot 2026-01-07 183502" src="https://github.com/user-attachments/assets/5f9d1314-4761-4b07-9649-d784f388ae91" />

</p>

<p>
<img width="439" height="563" alt="Screenshot 2026-01-07 183529" src="https://github.com/user-attachments/assets/2f4672be-80b1-4898-a16f-df702aa8c316" />

</p>

<p>
<img width="478" height="577" alt="Screenshot 2026-01-07 183550" src="https://github.com/user-attachments/assets/2aaa23bc-d62a-49d5-bbc7-7fa555c3dd9a" />

</p>

<p>
<img width="482" height="574" alt="Screenshot 2026-01-07 183557" src="https://github.com/user-attachments/assets/3a592f28-2776-4de0-8a43-b1f5b093f7ac" />

</p>

<p>
<img width="444" height="587" alt="Screenshot 2026-01-07 183610" src="https://github.com/user-attachments/assets/6c7bc91b-ce96-444c-a1e9-87e96e89a9f0" />

</p>

<p>
<img width="405" height="497" alt="Screenshot 2026-01-07 183905" src="https://github.com/user-attachments/assets/fe97078b-be4b-46a2-ad18-e6aa936427ae" />

</p>

<p>
<img width="459" height="446" alt="Screenshot 2026-01-07 183926" src="https://github.com/user-attachments/assets/c8b9308f-a444-41f0-b4f0-faaea3fb4bb8" />

</p>
<br />

<h3> Step 3: Join Client-1 to your domain (mydomain.com)</h3>

- Login to Client-1 as the original local admin (labuser) and join it to the domain
(computer will restart)

- Login to the Domain Controller and verify Client-1 shows up in Active Directory Users and Computers (ADUC)
  
- Create a new OU named “_CLIENTS” and drag Client-1 into there


<br />
<p>
<img width="2051" height="525" alt="Screenshot 2026-01-07 184232" src="https://github.com/user-attachments/assets/a9c7ab53-f803-43ce-b363-354182729e5f" />

</p>

<p>
<img width="413" height="265" alt="Screenshot 2026-01-07 184259" src="https://github.com/user-attachments/assets/724d7044-05e6-4d52-b8e0-8426b120de3b" />

</p>

<p>
<img width="460" height="421" alt="Screenshot 2026-01-07 184313" src="https://github.com/user-attachments/assets/2eaece23-441d-4f3d-bc6e-00d21800cb11" />

</p>

<p>
<img width="1196" height="920" alt="Screenshot 2026-01-07 184815" src="https://github.com/user-attachments/assets/0858d8fe-30e1-44de-8504-e4ac4dbba63a" />

</p>

<p>
<img width="1038" height="557" alt="Screenshot 2026-01-07 184843" src="https://github.com/user-attachments/assets/a030f276-bdda-4891-ad47-d1f84bf186c0" />

</p>

<p>
<img width="434" height="491" alt="Screenshot 2026-01-07 184924" src="https://github.com/user-attachments/assets/22849d6c-d0a5-4653-8062-a3d8ae5bff0f" />


</p>

<p>
<img width="486" height="322" alt="Screenshot 2026-01-07 185108" src="https://github.com/user-attachments/assets/0a185ca7-3987-426d-8c54-4251b91d156c" />

</p>

<p>
<img width="300" height="179" alt="Screenshot 2026-01-07 185121" src="https://github.com/user-attachments/assets/a50df264-20af-4993-9059-5355bf5570da" />

</p>

<p>
<img width="357" height="189" alt="Screenshot 2026-01-07 185132" src="https://github.com/user-attachments/assets/1b5c91c9-a165-44c3-a46d-16442d6b6851" />

</p>

<p>
<img width="351" height="173" alt="Screenshot 2026-01-07 185159" src="https://github.com/user-attachments/assets/2e35812a-5afe-4299-94c5-4eae935eab5b" />

</p>

<p>
<img width="835" height="702" alt="Screenshot 2026-01-07 185251" src="https://github.com/user-attachments/assets/82d25b0d-3b37-4123-aae7-60902ea30ca2" />

</p>

<p>
<img width="827" height="685" alt="Screenshot 2026-01-07 185258" src="https://github.com/user-attachments/assets/954a9045-8323-40e2-a3fd-c5d6042d5720" />

</p>

<p>
<img width="1222" height="536" alt="Screenshot 2026-01-07 185356" src="https://github.com/user-attachments/assets/653ee335-baeb-4e14-a4b8-c248fd2debbd" />

</p>

<p>
<img width="1226" height="570" alt="Screenshot 2026-01-07 185412" src="https://github.com/user-attachments/assets/b206b09f-6f76-47d1-9a34-84e5a400da51" />

</p>

<p>
<img width="1231" height="560" alt="Screenshot 2026-01-07 185453" src="https://github.com/user-attachments/assets/ca5ad165-1f98-4e12-8857-65fc35b3f8f5" />

</p>

<p>
<img width="545" height="563" alt="Screenshot 2026-01-07 185521" src="https://github.com/user-attachments/assets/fbaaf2b4-c68d-4355-bbf6-e80599753c45" />

</p>

<p>
<img width="1252" height="576" alt="Screenshot 2026-01-07 185554" src="https://github.com/user-attachments/assets/6bf8207b-f914-4d43-b910-271c8a02e056" />

</p>

<p>
<img width="1225" height="561" alt="Screenshot 2026-01-07 185714" src="https://github.com/user-attachments/assets/f347aa0c-0af4-4444-b55d-b2835abd71c6" />

</p>

<p>
<img width="1229" height="563" alt="Screenshot 2026-01-07 185722" src="https://github.com/user-attachments/assets/212b723d-957b-4d78-a8b3-44942eac0a45" />

</p>
<br />

<h3> Step 4: Setup Remote Desktop for non-administrative users on Client-1</h3>

- Log into Client-1 as mydomain.com\jane_admin
  
- Open system properties
  
- Click “Remote Desktop”

- Allow “domain users” access to remote desktop

- You can now log into Client-1 as a normal, non-administrative user now

<br />
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<h3> Step 5: Create a bunch of additional users and attempt to log into client-1 with one
of the users</h3>

- Login to DC-1 as jane_admin

- Open PowerShell_ise as an administrator

- Create a new File and paste the contents of the script into it

- Run the script and observe the accounts being created

- When finished, open ADUC and observe the accounts in the appropriate OU
(_EMPLOYEES)

- Attempt to log into Client-1 with one of the accounts (take note of the password in
the script)


<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

