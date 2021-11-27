# UTS-Sistem Administrasi Server
------
## Rachmad Saflyi    IT0201
------
**Question**
------
<img width="461" alt="bbbb" src="https://user-images.githubusercontent.com/92350603/143621126-49a7a818-0d3d-4a3f-b737-ff4fafdae37f.PNG">

**Answer**
------
### A. Instalasi windows server 2022

Download ISO Installer windows server 2022

   https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2022
   
   Select download the `ISO` then follow it step by step.
   
   <img width="874" alt="cccc" src="https://user-images.githubusercontent.com/92350603/143621513-6da949ad-311d-4c4b-af20-f8dc3031a9e4.PNG">

- Then open Oracle VM
  
  Enter the name of the machine and type of system to use
![Screenshot (512)](https://user-images.githubusercontent.com/93419670/143677833-6a3f5c7e-c4cb-41d9-9bad-47d9834f3ba6.png)

- Define ram, create the disk defining type and size
![Screenshot (512)](https://user-images.githubusercontent.com/93419670/143677853-0d5a25b4-4702-45f2-a146-93ec03956534.png)
![Screenshot (514)](https://user-images.githubusercontent.com/93419670/143677864-1f8c63db-b951-4840-b2ac-e6b35e4f6083.png)
![Screenshot (515)](https://user-images.githubusercontent.com/93419670/143677869-b53cb0b4-12ca-48e7-937a-e5631994d241.png)
![Screenshot (516)](https://user-images.githubusercontent.com/93419670/143677873-6e0c85a4-68f4-4cc5-9806-ee81bad7125e.png)
![Screenshot (517)](https://user-images.githubusercontent.com/93419670/143677880-90685cd2-9141-4988-8bd5-e211de799dde.png)
![Screenshot (518)](https://user-images.githubusercontent.com/93419670/143677888-6ef87121-3bbe-4288-8b3f-6042b4669d44.png)

- Go to the machine configuration and in the `Network` section set `Bridge adapter`
![Screenshot (519)](https://user-images.githubusercontent.com/93419670/143677903-8e67b359-ed26-4915-8d16-f5600af654b0.png)

-  Click on `Start` and select the `ISO downloaded`
![Screenshot (520)](https://user-images.githubusercontent.com/93419670/143677928-0e3fee01-1f0d-449e-bce3-5f5eb8d3c85a.png)


-  Click on `Start` and the Windows Server 2022 installation wizard will load
![Screenshot (464)](https://user-images.githubusercontent.com/93419670/143677946-5ec8d35a-a6e0-4484-a865-3193fbaf2140.png)

-  Click on `Install now`
![Screenshot (465)](https://user-images.githubusercontent.com/93419670/143677951-e6e1e0b2-281b-4f76-9fff-0514c8d59aae.png)


- Select windows server 2022 desktop experience
![Screenshot (467)](https://user-images.githubusercontent.com/93419670/143677956-8429e8c4-08c3-4438-b596-fed7458c838c.png)


- Accept the license and then proceed with the installation of Windows Server 2022
![Screenshot (468)](https://user-images.githubusercontent.com/93419670/143677961-c9b41d6e-2b8c-49f1-9913-75db500b8993.png)

- Location installation of windows server 2022
![Screenshot (469)](https://user-images.githubusercontent.com/93419670/143677985-38b28c3a-553e-4c76-87b1-82ca9356bc4f.png)

- Next, custom your password administrator
![Screenshot (484)](https://user-images.githubusercontent.com/93419670/143678000-d6a76d8c-d9b0-4938-b7bf-40da3ba6b2b5.png)

- Access the menu `Input – Keyboard – Insert Ctrl + Alt + Del`. Enter the password created and wait for the configuration to load
![Screenshot (485)](https://user-images.githubusercontent.com/93419670/143678006-a2456a55-49b5-448b-8eac-d5109ee2e1a5.png)
![Screenshot (486)](https://user-images.githubusercontent.com/93419670/143678011-3cd301f5-6e92-4065-8200-dc6842f21f05.png)

- Windows Server 2022 has been successfully installed
![Screenshot (488)](https://user-images.githubusercontent.com/93419670/143678042-5cc0cebd-ed7d-4bd7-98ef-74f6c6242550.png)
![Screenshot (489)](https://user-images.githubusercontent.com/93419670/143678047-4e3c41ed-705c-4139-bd10-a6829b64f022.png)


### B. Instalasi Active Directory Domain Services
-  Before doing the installation, we change the computer name first by going to windows powershell.
   Then type `rename-computer -Newname Server2022`
      - Open the start menu and select `Windows PowerShell`
  ![Screenshot (490)](https://user-images.githubusercontent.com/93419670/143678082-99ec7459-09d3-4548-8fed-2f0371574cb7.png)
![Screenshot (492)](https://user-images.githubusercontent.com/93419670/143678087-fc54276f-5c1f-4dfe-9d07-0c516697dab0.png)
![Screenshot (493)](https://user-images.githubusercontent.com/93419670/143678092-0f7313e4-91e5-43d9-a6ae-ec38c08caefe.png)
![Screenshot (494)](https://user-images.githubusercontent.com/93419670/143678093-3cd5a9c1-1062-4583-b4f2-6cf8940909f4.png)

      - Then Restart, and open`Server Manager` 
  ![Screenshot (495)](https://user-images.githubusercontent.com/93419670/143678106-e7266f96-189b-42f1-ac52-1b352ce1d4a4.png)

      - Select Menu `manage`, Then `Add Rules and Features` 
   ![Screenshot (496)](https://user-images.githubusercontent.com/93419670/143678115-5f5aa534-bf0f-4a51-9149-1458d7292ce6.png)

      - Select Next
   ![Screenshot (497)](https://user-images.githubusercontent.com/93419670/143678131-a805a378-c64e-4ded-b6bd-c47d4f689780.png)

      - Select option`Role-based or feature-based installation`. And `Next`
   ![Screenshot (498)](https://user-images.githubusercontent.com/93419670/143678167-50552e47-da4c-49dc-b264-78b91c7d8c87.png)

      - Click `Select a server from the server pool` to select a local storage directory. Then `Next`
   ![Screenshot (499)](https://user-images.githubusercontent.com/93419670/143678174-32e09375-c8e3-4e98-9d7f-39984c00cedb.png)

      - Next, put a check mark in the `Active Directory Domain Services` box. When you check the box, on the right appears 
        a brief description of ADDS and how it works. Then click `Add Features`.
   ![Screenshot (500)](https://user-images.githubusercontent.com/93419670/143678207-899b7394-01b1-474a-a63b-f8c2e0f499f9.png)
   ![Screenshot (501)](https://user-images.githubusercontent.com/93419670/143678209-45eabc44-7ce4-40aa-9bd3-59d29c8b6487.png)

   
   
### C. Instalasi DNS server
   - We need to install and configure the Active Directory role and DNS server to work together.
     Checklist `DNS Servers` then `add features` 
   ![Screenshot (503)](https://user-images.githubusercontent.com/93419670/143678288-41813f5d-8168-4d20-aa79-b14288936fa3.png)
![Screenshot (502)](https://user-images.githubusercontent.com/93419670/143678292-6a5149c4-7a12-405d-9376-b57ecad3701a.png)



### D. Instalasi Net Framework 3.5
   - Checklist `.NET Framework 3.5 features`
   ![Screenshot (505)](https://user-images.githubusercontent.com/93419670/143678326-820cb414-bdaf-4b0e-b96a-3c0a1d656899.png)


   - Click `Next`
   ![Screenshot (507)](https://user-images.githubusercontent.com/93419670/143678352-f4182c1c-c020-4f22-a564-21ff6e2e63c4.png)


   - Click `Next`again
   ![Screenshot (508)](https://user-images.githubusercontent.com/93419670/143678356-0e2dc61d-82a3-44d5-ac40-2386331e9ccb.png)


   - Select `Install`
   ![Screenshot (509)](https://user-images.githubusercontent.com/93419670/143678360-4713fe29-fc12-4251-8e5e-6d9a3935f632.png)


### E. Promote Server to a Domain Controller
