### MGMT 10.129.129.0/24
- IPv6-SRV1/ether8 10.129.129.1
- WAN1/MGMT1 10.129.129.1
- AGG1/MGMT1 10.129.129.2
- CPE1/ether8 10.129.129.3
- CPE2/ether8 10.129.129.4

### IPv6 Supernet
fdd6:8e83:ceb9::/48
- fdd6:8e83:ceb9::/49
  - fdd6:8e83:ceb9::/64 - Loopbacks (as /128)
    - IPv6-SRV1 - fdd6:8e83:ceb9::1/128
    - WAN1 - fdd6:8e83:ceb9::2/128
    - AGG1 - fdd6:8e83:ceb9::3/128
#### PTPv6
  - fdd6:8e83:ceb9:1::/64 - Point-to-point links (as /126)
    - fdd6:8e83:ceb9:1::/126 - IPv6SRV/ether1 fdd6:8e83:ceb9:1::1/126 - fdd6:8e83:ceb9:1::2/126 WAN1/eth2
    - fdd6:8e83:ceb9:1::4/126 - WAN1/eth1 fdd6:8e83:ceb9:1::5/126 - AGG1/eth1 fdd6:8e83:ceb9:1::6/126
    - fdd6:8e83:ceb9:1::8/126 - AGG1/eth3 fdd6:8e83:ceb9:1::9/126 - CPE2/ether1 fdd6:8e83:ceb9:1::a/126
    - fdd6:8e83:ceb9:1::c/126 - AGG1/eth2 fdd6:8e83:ceb9:1::d/126 - CPE1/ether1 fdd6:8e83:ceb9:1::e/126
    - fdd6:8e83:ceb9:1::10/126
    - fdd6:8e83:ceb9:1::14/126
    - fdd6:8e83:ceb9:1::18/126
    - fdd6:8e83:ceb9:1::1c/126  
  - fdd6:8e83:ceb9:8000::/49 - Client delegations (as /56)

### LOOPBACK
- BLOCK 10.255.255.0/24
  - IPv6-SRV1 - 10.255.255.1
  - WAN1 - 10.255.255.2
  - AGG1 - 10.255.255.3


### PTPv4 10.2.2.0/24
- BLOCK 10.2.2.0/30 - IPv6SRV/ether1 10.2.2.1/30 - WAN1/eth2 10.2.2.2/30
- BLOCK 10.2.2.4/30 - WAN1/eth1 10.2.2.5/30 - AGG1/eth1 10.2.2.6/30
- BLOCK 10.2.2.8/30 - AGG1/eth3 10.2.2.9/30 - CPE2/ether1 10.2.2.10/30
- BLOCK 10.2.2.12/30 - AGG1/eth2 10.2.2.13/30 - CPE1/ether1 10.2.2.14/30
- BLOCK 10.2.2.16/30 -
