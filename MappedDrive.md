# Mapped Drive Configuration
- The mapped drive feauture was created to demonstrate role-based access control
- A shared folder was created and NTFS permissions configured to allow only finance group users and administrators
  

  ## NTFS Configuration
  - **Finance Group**: Modify access
  - **Domain Admins**: Full control
  - **system and Creator Owner**: Full contol
  - **Everyone**: Removed
  
   A GPO was used to map the folder as a network drive

     <img width="750" height="400" alt="map-drive" src="https://github.com/user-attachments/assets/7dfa560c-bf7d-49cb-9ef7-be428641519d" />

  GPO was then linked to all User OUs to test access control

  ## Access testing
   **Finance group user**: Drive Mapped, folder accessible
  
  
   
     <img width="750" height="400" alt="Screenshot jdoe" src="https://github.com/user-attachments/assets/3e513759-b5d4-4f26-8e7d-c34767d16f6b" />


   **Non Finance Group User**: Drive Mapped,folder Access Denied

  
   
   
     <img width="750" height="400" alt="tsmali" src="https://github.com/user-attachments/assets/63abe65b-84b1-45b9-a1fb-9f4825f041cc" />

