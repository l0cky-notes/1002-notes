ipconfig 
	most of your troubleshooting starts with your IP addr
		ping your local router/gateway
	determine TCP/IP and network adater information
		and some add IP details

ping 
	test reachability
		determine round-trip time
		use internet control message protocol (ICMP)
	one of your primary troubleshooting tools
		can you ping the host?
	writtenn by mike muuss in 1983
		the sound made by sonar
		not an acronym for packet INternet groper
			a backronym

tracert
	determine the route a packet takes to a destination
		map the entire path
	takes advantage of ICMP time to live exceeded error message
		the time in TTL refers to hops, not seconds or minutes
		TTL=1 is the first router, TTL=2 is the second router, etc
	not all devices will reply with ICMP time exceeded message
		some firewalls filter ICMP
		ICMP is low-priority for many devices


flavors of traceroute 
	not all traceroute are the same
		minor difference in the transmitted payload
	windows commonly sends ICMP echo requests
		receives ICMP time exceeded message
		and an icmp echo reply from the final/destination devices
		unfortunately, outgoing ICMP is commmonly filtered

	some os allow you to specify the protocol used
		linux, Unix, macOS, etc
	ios devices send UDP datagrams over port 33434
		the port number can be changed with extended options
		
netstat
	network statistics
		many different OS 
	netstat -a 
		show all active connections
	netstat -b 
		show binaries (windows)
		requires elevation
	netstat -n
		do not resolve names

nslookup
	look info from DNS server
		canonical, IP address cache timers, etc
	lookup names and IP addr 
		many different options
		
		
common Net commands 
	view network resources
		net view \\<servername>
		net view /workgroup:<workgroupname>
	map a network share to drive letter
	net use h: \\<servername>/<sharename>
	view user accout info and reset password
	net user <username>
	net user <username> * /domain