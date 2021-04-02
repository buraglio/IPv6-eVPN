Important Notes and Caveats:

1. Routed interfaces are built as raw ports, not vlans. This is typically not best practice and is only for prototyping purposes.
2. Address Plan is fairly simplistic, probably could use some more TLC.
3. Point-to-points are built as /30 and /126 in order to avoid (possibly now resolved) Mikrotik issues with /31 and /127 subnets.
4. It is assumed that OSPF is the IGP as Mikrotik does not (yet?) support IS-IS =(
5. Certain Jericho based platforms require some TCAM provisioning. "hardware tcam profile vxlan-routing" 
