# IPv6-eVPN

### Multi-Vendor IPv6 eVPN configuration lab
Included here are basic lab configurations for Mikrotik and Arista testing using Arista as backbone routers and Mikrotik as both CPE and an IPv6 DHCP-PD server as well as the Topology and Eve-NG Lab XML File. This lab should provide a foundation for eVPN isolation of CPE with IPv6 connectivity and should be suitable as a basis for building an ISP using such techniques.

### Files and such

1. IPv6-eVPN-Lab.unl - the Eve-NG XML file that is the lab
2. CPE - Mikrotik CPE devices obtaining a DHCPv6-PD
3. IPv6-SRV1 - Mikrotik instance providing DHCPv4/6-PD
4. AGG1 - Arista Aggregation device (i.e. a regional or localish aggregation router and eVPN aggregator)
5. WAN1 - Arista upstream router representing a WAN segment or set of segments

### Usernames and Access
Yes, the secrets are in the configurations. You can cut and paste the configurations into your lab directly. All devices use admin/admin as the username and password. 

### Diagrams and physical layout

The Physical layout of this test environment is detailed in this diagram. The virtualization platform used is an Eve-NG system running on bare metal but given the limited resources needed for both Mikrltik and vEOS this could probably be pushed into a nested virtualization sytem (Eve-NG VM inside something like proxmox or vmware). It could also be deployed on bare metal if one were so inclined, but interfaces configurations might need to be adjusted.

The physical topology inside of eve-ng that comprises the test network looks roughly like this.  
![Virtual Router Topology](https://github.com/buraglio/IPv6-eVPN/blob/c2056f97eee416a4113939cbb0aa29860d9cc436/IPv6%20eVPN%20Lab.png "Virtual Router Topology")
