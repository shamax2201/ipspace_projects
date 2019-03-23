# ipspace_projects
Includes all the assignments for ipspace hands-on module

###Physical Lab setup information
All Network Devices (Routers and Switches) are run on GNS3, which is hosted on VMware Workstation running on a physical PC (with 64 GB of RAM)
####Network Devices
- All virtual Routers used in the LAB are CSR1000v running csr1000v-universalk9.03.17.00.S.156-1.S-ext.qcow2 image
- All virtual Switches used in the LAB are running IOSvL2  running vios_l2-adventerprisek9-m.03.2017.qcow2 image
####Ansible Host
- Ansible is run on a virtual Centos6.9 box hosted on the same  VMware Workstation as the GNS3.

##Lab Topology

![alt text](https://www.lucidchart.com/publicSegments/view/6d9e3904-0bc5-4cca-9e39-872d05f06c29/image.png)

The lab comprises of an MPLS network with two 2 x P Routers, 4 x PE Routers (all connected to both P routers) and 4 x Switches, connected to each PE routers.
All Routers and Switches will have one interface (used as the Mgmt Interface) connected to Virtual OOB switch (which is a GNS3 included basic switch). 
The OOB Switch is also connected to a GNS3 included "Cloud connector" device which is bridging with the PC's LAN Nick.
The sam LAN is also bridging with the NIC attached to the Ansible host VM.

The Management IP Addressing is as follows
  
    - P1:   10.10.1.51
    - P2:   10.10.1.51
    - PE1:  10.10.1.61
    - PE2:  10.10.1.62
    - PE3:  10.10.1.63
    - PE4:  10.10.1.64
    - SW1:  10.10.1.71
    - SW2:  10.10.1.72
    - SW3:  10.10.1.73
    - SW4:  10.10.1.74
    - Ansible Host : 10.10.1.246



 

