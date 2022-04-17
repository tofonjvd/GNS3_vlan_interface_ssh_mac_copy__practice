In this topology, we are going to work on configuring:
+ IP addresses on end devices
+ VLAN on switches
+ SSH on switches
+ MAC address table on switches
+ VTP mode on switches
+ Trunk ports on switches
You can find other necessary information in the topology file.
So fasten your seatbelts cause we have tons of
commands to issue !


Tasks you must achive :
+ Configuring PC1 - PC8 IP addresses based on
giving information below each computer
+ Configuring each switch's Hostname based on the
name of that switch ( for example, S1's hostname should
be "S1", and so on )
+ Assign each computer to the related VLAN ID
based on giving information below each computer
+ Configuring a VLAN interface on each switch
based on giving information for each switch ( notice
that the interface number must be "VLAN 1" and the IP address for the
related switch is "192.168.1" + switch's index. For example, the IP address
for S3's interface vlan 1 is "192.168.1.3", and the subnet mask for all switches
is 255.255.255.0 )
+ Configuring SSH for each switch based on information below: 
	- Username should be equal to the switch's hostname.
	This means for example the username for S1 is "s1" and so on
	- The password for all switches is "admin"
	- Notice that you must only open SSH connections for "line vty
	0 to 4". Moreover, you must block other input connections and
	again, only open the SSH connections ( Hint: by using "transport"
	command )
	- The domain name for all switches is "home.com"
	- The Login mode should be set to "local" for all switches
	- Set the enable password for each switch to "admin"
	- Use scrypt or SHA algorithm for your passwords ( optional task )
+ Configuring interfaces 3/0 and 3/1 for all switches to trunk mode with
the dot1q encapsulation. ( Hint: use "range" command )


After configuring all of the taske, you should issue these "show" commands and analyse the output by yourself
for the sake of comprehending the commands and changes.
+ show mac address-table
+ show mac address-table dynamic vlan [vlan-id]
+ show mac address-table count
+ show crypto key mypubkey rsa
+ show ip ssh
+ show ssh
The list is not limited to here, there are tons of other "show" commands that you can issue, so keep going...

Bonus task :
You can issue the "show running-config" and "show startup-config" and compare them together, then you can
issue the "copy running-config startup-config" to save the configurations in the NVRAM
and see how Cisco IOS work with it's storages. Also remember to save the configurations on the PCs.

Good Configing !
