# active-directory-homelab
A comprehensive Active Directory homelab built on Hyper-V featuring Windows Server 2022 as a Domain Controller and Windows 10 Pro clients. Includes full AD DS configuration, DNS setup, user/group management, and Group Policy Objects for hands-on learning and testing. Planning to change network Adapter later to private switch to implement DHCP

## Infrastructure
- **Hypervisor:** Microsoft Hyper-V
- **Domain controller:** Windows Server 2022
- **Client Workstation:** Windows 10 pro
- **Network:** External Virtual Switch

## Server Configuration
- windows Server 2022 installed
- Static IP for Server Configured with DNS pointing to itself
- AD DS role installed and promoted to Domain Controller
- DNS verified with foward lookup zones
  
  - ![Server Network configuration(Static IP)](server-configuration-network.md)
  - ![Active Directory Doamain Services installation](adds-installation.md)

### Active Directory Configuration
- Implemented a structured OU design to improve organization and scalabilty
- Created security groups aligned with departmental roles
- Applied group-based management to support access control and policy assignment
  
  - ![Active Directory configuration](Ad-configuration-OUs-groups.md)

### Client Workstation Configuration
- Configured a Windows 10 Pro client Workstation and joined it to the Active Directory Domain
- Verified successiful domain join for GPO application and testing
  
  - ![client workstation configuration](client-domain-join.md)

## Group Policy configuration and testing
- Created and applied Group Policy Objects(GPOs) to manage and configure users and computers's settings within Domain
- Linked GPOs to appropriate OUs and verified policy enforcement on the Domain joined workstation

  - ![GPO configuration and application](gpo-testing.md)




  
