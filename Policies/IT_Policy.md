*This is just an example document and should be reviewed by your network admin, CTO, or the person who handles IT at your company.  DO NOT JUST COPY PASTE THIS. Make sure you can actually comply with it. 

1	Overview and Objective

This document sets out [INSERTCOMPANYNAMEHERE] (“COMPANY”) policy on how it will design, manage, and support computer networks. Its intended audience is IT and information security management and support staff who will implement and maintain the organization’s defenses. Additionally, this policy establishes the standards and procedures for maintaining proper access security at COMPANY. It addresses:

•	Definition of process owners and their responsibilities
•	User access rights
•	Annual review of access and segregation of duties and approval by the process owners

2	Scope

This policy applies to all systems, people, and processes that constitute the organization’s information systems, including board members, directors, employees, suppliers, and other third parties who have access to COMPANY systems. 

3	 Network Security Policy

The use of networks is an essential part of the day to day business of COMPANY. Networks not only connect many of the components of business processes together internally, but they also link the organization with its suppliers, customers, and stakeholders.

The fact that so much information runs through our networks makes them a target for those who would try to steal that information and disrupt our business. Therefore, these networks need to be protected to ensure that the confidentiality, integrity, and availability of our vital information is assured at all times.

The effective protection of our networks requires that we adopt good practices in information security covering the design, implementation, operation, and management of them and that we ensure that everyone involved follows these practices.

This policy sets out COMPANY rules and standards for network protection and acts as a guide for those who create and maintain our IT infrastructure.

Network Security Design

The design of networks is a complicated process requiring a good knowledge of network principles and technology. Each design is likely to be different, based on a specific set of requirements that are established early on in the process. This policy does not attempt to specify how individual networks should be designed and built. Moreover, this policy provides guidance for the standard building blocks that should be used.

Requirements

A network design should be based on a clear definition of requirements which should include the following security-related factors:

●	The classification of the information to be carried across the network and accessed through it
●	A risk assessment of the potential threats to the network, taking into account any inherent vulnerabilities
●	The level of trust between the different components or organizations that will be connected
●	The hours of availability and degree of resilience required from the network
●	The geographical spread of the network
●	The security controls in place at locations from which the network will be accessed
●	Security capabilities of existing computers or devices that will be used for access 

Defense in Depth

A “Defense in Depth” approach will be adopted to network security whereby multiple layers of controls are used to ensure that the failure of a single component does not compromise the network. For example, network firewalls should be supplemented by host-based software firewalls on servers and clients in order to provide several levels of firewall protection.

At key points in the network, a “defense diversity” approach should also be taken so that vulnerabilities are minimized. For example, this may involve using firewalls from different vendors in series so that if a vulnerability is exploited in one device, the other will not be subject to it. This may be extended to the use of more than one network virus scanner at the perimeter for the same reason.

Network Segregation

The principle should be adopted that a network should consist of a set of smaller networks segregated from each other based on either trust levels or organizational boundaries (or both).  

For a large network, this should be achieved using separate domains, particularly where separate organizations’ networks are being linked. An appropriate level of trust should be configured at the domain level and domain perimeters should be secured using a firewall where appropriate.

Within networks, Virtual Local Area Networks (VLANs) will be used to segregate organizational units.

Perimeter Security

At all perimeters between the internal network and an external network (such as the Internet), effective measures should be put in place to ensure that only authorized network traffic is permitted. This will usually consist of at least one Stateful Inspection firewall and for major links with the Internet, an Application (or Application Gateway) firewall should be used. For connections such as broadband at smaller locations, a Packet Filtering firewall may suffice, depending on the results of a risk assessment.  

Servers that are intended to be accessed from an external, insecure network (such as web servers) should be located in a Demilitarized Zone (DMZ) of the firewall in order to provide additional protection for the internal network.

Public Networks

Where information is to be transferred over a public network such as the Internet, strong encryption via SSL must be used to ensure the confidentiality of the data transmitted.

Servers that will be accessed from devices on the public network will be located in the DMZ of the firewall.

Wireless Networks

Wireless networks should be secured using WPA2 encryption. WEP and WPA should not be used.

Wireless networks should be treated as insecure even if WPA2 is used as the encryption method and a firewall installed between the wireless network and the main LAN.

A guest wireless network may be provided for visitors. This should be physically separate from all internal networks (including internal wireless networks) and also secured using a firewall.

Wireless access points should be configured to not broadcast their SSID and to not allow secure connection using WPS (Wi-Fi Protected Setup) via physical access to the access point itself.

Wireless access point admin login passwords should always be changed from the default.

Physical Security

Remote network equipment will be housed in secure cabinets which will be locked at all times. Only support staff will have access to the key to each cabinet. 

Backbone and centralized network equipment will be housed in appropriate lockable cabinets or racks in a secure server room to which only authorized support staff will have access (with the exception of local facilities staff for reasons of health and safety).

Wireless access points located in public areas should be hidden from view where possible and should be placed in positions where access by the public is difficult (e.g. in or near the ceiling).

Remote Access

Where there is a requirement for remote access to the internal network the following controls will be used:

●	A Virtual Private Network (VPN) will be used providing session encryption using SSL
●	Two-factor authentication at the client where appropriate
●	Network Access Control (NAC) will be used to restrict access to remote clients that do not meet minimum requirements (e.g. virus control)

Remote access should be granted on an “as required” basis rather than for all users by default.

Network Intrusion Detection

A Network-based Intrusion Detection System (NIDS) should be installed at the network perimeter and at all key points within the network (e.g. on critical servers).

For networks with high-security requirements, an Intrusion Prevention System (IPS) should be considered, although its implementation should be approached with caution to avoid a high degree of false positives with the corresponding disruption to service to users.

Network Security Standards

The following standards will be adopted with respect to network configuration and security. 

Network Hardware

Where possible a single supplier policy will be used for network hardware. An exception will be made where the use of multiple vendor hardware may increase the level of security provided (e.g. in a dual network-based firewall configuration).

Network routing will be based on [Cisco] routers using OSPF. [Cisco Gigabit] switches will be used as a standard for connectivity.  Switch ports, including diagnostic ports, will be configured to be administratively disabled until required. Hubs will not be used due to their inherent security weaknesses.

Cat 6 UTP will be used for network cabling unless specific circumstances (such as excessive interference) preclude its use. The network topography used will be Ethernet according to the IEEE 802.3 family of standards.

Network Protocols

The protocol used on all networks will be TCP/IP. UDP will be used where appropriate but other OSI layer 4 network protocols should not be used.

Only protocols and ports required on a specific server should be enabled by default in order to reduce the attack surface. This is especially true for servers within the DMZ of the firewalls.

Network Security Management

Once networks have been designed and implemented based on a clear set of security requirements, there is an ongoing responsibility to manage and control the secure networking environment to protect the organization’s information in systems and applications. This should be achieved via controls in the following areas.

4	Roles and Responsibilities

Roles and responsibilities for the management and control of networks should be clearly defined.  On an annual basis, IT will conduct a re-certification process of system access security rights to ensure that the appropriate users are authorized for the functions or transactions of the proper system.
The respective process owners will review and validate access data. If access modifications become apparent as a result of the re-certification process, IT Access Forms will be completed as appropriate prior to any modifications being made within the system.

The CTO will periodically conduct a review with the respective process owner to determine that proper segregation of duties has been achieved within selected system responsibility groups. 

Logging and Monitoring

Logging levels on network devices should be configured in accordance with organization policy and logs monitored on a regular basis.

Firewall logs will be monitored for signs of excessive port scanning which may be a precursor to a remote attack. Where installed, a Network-based Intrusion Detection System should be configured to alert the Network Operations team of this activity. 

Network monitoring for availability should be achieved using an appropriate SNMP-based network management tool OpManager and Manage Engine Event Log Analyzer, and recovery actions automated where possible.  

Network Changes

All changes to network devices will be subject to the change management process and appropriate risk assessment, planning, and back-out methods put in place. The Configuration Management Database (CMDB) should be updated whenever such changes are carried out so that a current and accurate picture of the network is maintained at all times. 

Network Security Incidents

Events which are deemed to be network security incidents should be recorded and managed accordingly.

Major network outages should be managed with a higher degree of caution and, where appropriate, should include the invocation of aspects of the business continuity plan.

5	Conclusion

Network security is a cornerstone of COMPANY’s defenses against many of the threats with which we are faced. Only by designing effective security into every new system and network from the very beginning can effective control be maintained and risk minimized. Further to this, additional controls must be implemented which ensure that proper segregation of duties is achieved and changes to the network environment happen in a well-managed manner.

Combined with watchful monitoring of the network itself and the tools put in place to manage it, this should ensure that the number and severity of network security incidents are minimized and our exposure from those that do occur is not as great as it otherwise might have been.

