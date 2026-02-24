# Enterprise-Hyper-V-High-Availability-Lab-Nested-Virtualization-
Enterprise-grade Hyper-V High Availability lab built with nested virtualization. Simulates Active Directory, DNS, Kerberos Live Migration, iSCSI shared storage, and Failover Clustering. Deployed on Windows 11 using VMware Workstation to replicate a production-style data center environment.

Architecture :

Windows 11 Host

└── VMware Workstation

      ├── DC01 (Domain Controller + DNS)
      
      ├── SRV01 (Hyper-V Host 1)
      
      ├── SRV02 (Hyper-V Host 2)
      
      └── STORAGE01 (iSCSI Target Server)
..........................................................................      
Technologies Used:
Windows Server 2019
Active Directory Domain Services
DNS (Forward & Reverse Lookup Zones)
Hyper-V
Kerberos Authentication
Constrained Delegation
iSCSI Target Server
Failover Clustering
Cluster Shared Volumes (CSV)
Nested Virtualization
...........................................................................
🚀 Implemented Features
1️⃣ Active Directory Infrastructure : 

Domain creation (corp.local)

DNS configuration (Forward & Reverse zones)

Secure Channel validation

SPN verification

2️⃣ Hyper-V Deployment :

Hyper-V installation on two hosts

Virtual Switch configuration

Network profile correction (DomainAuthenticated)

Firewall hardening for RPC, WMI, and Live Migration

3️⃣ Kerberos Live Migration :

Configured Constrained Delegation

Registered required services:

Microsoft Virtual System Migration Service

CIFS

Resolved Double Hop problem

Successful Live Migration between SRV01 and SRV02

4️⃣ Shared Storage (iSCSI) :

Deployed iSCSI Target Server

Created shared LUN

Connected Hyper-V hosts using iSCSI Initiator

5️⃣ Failover Clustering

Installed Failover Clustering role

Created Hyper-V Cluster Whith in SRV01

Added Cluster Shared Volume (CSV)

Enabled automatic VM failover 
............................................................................
🎯 Key Skills Demonstrated

Enterprise Infrastructure Design

Active Directory & DNS troubleshooting

Kerberos Delegation & SPN management

Hyper-V configuration & optimization

High Availability implementation

Storage configuration (iSCSI)

Network troubleshooting (RPC, Firewall, Network Profiles, )

Production-like virtualization design in nested environment.
..............................................................................
