# Group Policy creation and testing
- The following sections demonstrate how Group Policy Objects were configured and tested to enforce Domain standard and security controls
  
## GPO 1: Password and Account Lockout Policy
 - The following paswword and account lockout rules were enforced through the domain Group policy:
    - User must change password at next logon 
    - Minimum password length: **12 characters**
    - Password complexity: **Enabled** (uppercase,lowercase,numbers and special charcters)
    - Maximum failed logon attempts: **3**
    - Account lockout duration: **30 Minutes**
    - Account lockout trigered after exceeding the defined threshold
      
    ### Password policy verification
   -  To verify the correct policy application multiple user accounts were used on the client domain joined workstation
   -  Incorrect passwords were intentionally entered to generate failed logon attempts
   -  The user accounts were automatically lockedout confirming the policy enforment

    **Locked Account verification**
     - Locked-out Accounts were retrieved using powershell

       
       
       
   
  <img width="750" height="400" alt="lockedout-accounts" src="https://github.com/user-attachments/assets/908b0049-702d-48cd-aa20-450549439ee6" />



   **Locked-out Account Restoration**
    - Remediated locked-out accounts by resetting the passwords and unlocking accounts to restore user access

    
    
    
   
   <img width="750" height="400" alt="password-resets" src="https://github.com/user-attachments/assets/242633a3-46a2-4375-854a-20d99272a28f" />

## GPO 2: Destop Wallpaper Policy
- This policy was implemented to enforce a standardized desktop wallpaper for domain users and ensure a controlled desktop environment
- A custom test wallpaper was used to clearly verify the successful policy application on the client Workstation
- The policy defines the Wallpaper image location and enforces it to prevent users froms changing it

   ### Policy verification

  
    <img width="750" height="400" alt="wallpaper-display" src="https://github.com/user-attachments/assets/8c430d95-a7f3-428e-9e9a-d206495b22f7" />

## GPO 3: Control Panel Policy
- Configured a control panel and PC settings restrictions policy to apply to all standard Domain users excluding IT Admins
- This was to ensure that administrative users retain full system access for management and troubleshooting purposes
- The policy was linked to appropriate User OUs
- Policy was verified on the Domain joined workstation,the restriction  was successfully applied and  enforced as configured
  
  ### Policy Verification

  
    <img width="750" height="400" alt="PC -restrictions" src="https://github.com/user-attachments/assets/f00d6e6e-e437-4be8-baa7-0326282b7679" />

