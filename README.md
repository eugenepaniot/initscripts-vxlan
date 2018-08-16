Place these scripts in `/etc/sysconfig/network-scripts` on your
RedHat/CentOS/Fedora system.

Sample configuration for a `vxlan` interface:

	TYPE=VXLAN
	DEVICE=vxlan1000
	BOOTPROTO=none
	ONBOOT=yes
	TTL=255
	VNI=1000
	DSTPORT=4789
	LOCAL_ADDR="192.168.1.1"
	PHYS_DEV="eth0"
	OPTIONS="nolearning"
	BRIDGE="br1000"

