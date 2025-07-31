DHCP Server:

A DHCP Server is a network server that automatically provides and assignes IP addresses, default gateways, DNS servers, and other network parameters to client devices.
It allows devices to join the network without manual IP configuration.

Discover - client broadcasts a request to find a DHCP server.

Offer - DHCP server responds with IP offer

Request - client requests the offered IP

Ackowledge- DHCP server acknowledges and leases the IP to the clent.

Usage:

Home- Routers assign Ip's to phone, laptop

Office LAN's - automatically manage IP's for hundred's of employees

Data centers- Auto configure virtual machines

ISPs - Assign public IP's dynamically to users.

Hypervisor:

There are two main types of hypervisors

A hypervisor is a form of virtualization software used in Cloud hosting to divide and allocate the resources on various pieces of hardware. The program which provides partitioning, isolation, or abstraction is called a virtualization hypervisor. The hypervisor is a hardware virtualization technique that allows multiple guest operating systems (OS) to run on a single host system at the same time. A hypervisor is sometimes also called a virtual machine manager(VMM)

Types of Hypervisors:

TYPE-1 Hypervisor: 

The hypervisor runs directly on the underlying host system. It is also known as a "Native Hypervisor" or "Bare metal hypervisor". It does not require any base server operating system. It has direct access to hardware resources. Examples of Type 1 hypervisors include VMware ESXi, Citrix XenServer, and Microsoft Hyper-V hypervisor. 

Pros & Cons of Type-1 Hypervisor:

Pros: Such kinds of hypervisors are very efficient because they have direct access to the physical hardware resources(like Cpu, Memory, Network, and Physical storage). This causes the empowerment of the security because there is nothing any kind of the third party resource so that attacker couldn't compromise with anything. 

Cons: One problem with Type-1 hypervisors is that they usually need a dedicated separate machine to perform their operation and to instruct different VMs and control the host hardware resources.

 TYPE-2 Hypervisor: 
A Host operating system runs on the underlying host system. It is also known as 'Hosted Hypervisor". Such kind of hypervisors doesn’t run directly over the underlying hardware rather they run as an application in a Host system(physical machine). Basically, the software is installed on an operating system. Hypervisor asks the operating system to make hardware calls. An example of a Type 2 hypervisor includes VMware Player or Parallels Desktop. Hosted hypervisors are often found on endpoints like PCs.  The type-2 hypervisor is very useful for engineers, and security analysts (for checking malware, or malicious source code and newly developed applications).

Pros & Cons of Type-2 Hypervisor:

Pros: Such kind of hypervisors allows quick and easy access to a guest Operating System alongside the host machine running. These hypervisors usually come with additional useful features for guest machines. Such tools enhance the coordination between the host machine and the guest machine.

Cons: Here there is no direct access to the physical hardware resources so the efficiency of these hypervisors lags in performance as compared to the type-1 hypervisors, and potential security risks are also there an attacker can compromise the security weakness if there is access to the host operating system so he can also access the guest operating system.

 
