# Group Policy creation and testing
- The following sections demonstrate how Group Policy Objects were configured and tested to enforce Domain standard and security controls

## GPO 1: Destop Wallpaper Policy
- This policy was implemented to enforce a standardized desktop wallpaper for domain users and ensure a controlled desktop environment
- A custom test wallpaper was used to clearly verify the successful policy application on the client Workstation
- The policy defines the Wallpaper image location and enforces it to prevent users froms changing it

  
    <img width="750" height="400" alt="wallpaper-display" src="https://github.com/user-attachments/assets/8c430d95-a7f3-428e-9e9a-d206495b22f7" />

## GPO 2: Control Panel Policy
- Configured a control panel and PC settings restrictions policy to apply to all standard Domain users excluding IT Admins
- This was to ensure that administrative users retain full system access for management and troubleshooting purposes
- The policy was linked to appropriate User OUs
- Policy was verified on the Domain joined workstation,the restriction  was successfully applied and  enforced as configured
  
  ### Policy Verification

  
    <img width="750" height="400" alt="PC -restrictions" src="https://github.com/user-attachments/assets/f00d6e6e-e437-4be8-baa7-0326282b7679" />

