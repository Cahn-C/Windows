# Types of Network

## Workgroup
- No centralized authentication:
    - If you have 3 computers (computer 1, computers 2 and computer 3) you are user ```Jacob Roberts```, and you want to log into the computers, you will need to log into these computers from time to time.
    - Assuming that computer 1 is your primary computer, but you want to log into computer 3, someone will need to go to computer 3 and create a user account for ```Jacob Roberts```.
    - These computers have no relationship to each other than they physically reside on the same network.
- No centralized administration
    - If I want to configure the firewall, I have to physically touch each of these computers.
    - There is no place you can go and say, I want to configure this setting and I want it to apply to all 3 computers, this will not work due to the environment being workgroup.
- Max of 20 computers supported
    - Let's say that you have a shared folder on computer 1, and you want users on computer 2 and 3 to be able to browse to this share and copy a file, since there is just 2 computers, it is acceptable.
    - But let's say that there are 25 computers, if you have 25 different computers that try to browse the shared folder at the same time, they're going to get an error message that says "The maximum number of connections has been exceeded".
- Low security

<br>

## Domain
- Centralized authentication:
    - You have 3 computers (computer 1, computer 2 and computer 3), a server (Windows Server 2019 for example) that is configured with Active Directory domain services.
    - Once configured the server is now a domain controller.
    - Once you create the user ```Jacob Roberts``` and set the password, the user will be created to all 3 computers, because the 3 computers are all under the domain controller.
- Centralized administration:
    - If I wanted to block a certain application on all computers in the entire domain, I can go to my domain controller and use this utility called Group Policy.
    - With Group Policy, I can manage more than 3000 settings.
    - I can simply add a firewall rule that says block a specific application, and this will process out to all of the computers in my domain.
- Unlimited number of computers
- High security:
    - More simplistic to manage.

<br>

## Active Directory Domain Services(AD DS) Terms
AD DS is composed of both logical and physical components <br>
All Design components
- Logical Components
    - Domains
    - Domain Trees
    - Forests
    - OUs
    - Containers
<br>

All servers components <br>
- Physical Components
    - Domain Controllers: Server that has Active Directory domain services installed and configured.
    - Read-only Domain Controllers(RODC): Read only copy of Active Directory on it.
<br>

