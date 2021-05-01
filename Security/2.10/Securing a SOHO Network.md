ssid management
	service set id
		name of the wireless network
	change it to something not-so obvious
	disable SSID broadcasting
		ssid is easily determind 
		security through obscurity

wireless encryption
	all wireless computers are radio transmitters and receivers
		anyone can listen in
	ENCRYPT THE DATA
		password
	only people with the password can transmit and listen
		wpa2 encrption
	
power level controls
	usually a wireless config
		set it as low as you can 
	how low is low
		try different ones
	consider the receiver
		high-gain antennas can hear a lot
		locations locations
use WPS
	wi-fi protected setup
		originally called wi-fi simple config
	allows "easy" setup of a mobile devices
		A passphrase can be complicated to a novice
	different ways to connect
		pin on the devices
		butten
		nfc
		no USB
WPS hack
	pin is eight number
	easy to crack
	it takess about 4 hours

default username and passwords
	all access points have default username and password
		change yours
	the right credentials provide full control
		admin access
	very easy to find
		routerpasswords.com

mac address filtering
	media access control
		the "hardware" address
	limit access through the physical hardware address
		keeps the neighbors out
		add admin with visitors
	easy to find working MAC address through wireless LAN analysis
		mac address can be spoofed
		free open-source software
	security through obscuruty

ip address
	DHCP(auto) ip addressing or manual ip addressing
	ip address are easy  to see in an unencrypted network
	ip address are east to see in an unecrypted network
	if the encryption is broken, the ip will be obvious
	config a static ip address is not a security techniquew

soho firewalls
	soho app 
		geanerally has reduced throughput requirement
usually include multiple functions
	wap, router, firewall, content filter
may not provide advanced cap
	dynamic routing
	remote support
install the latest software 
	update and upgrade the firmware
	firewall, routing, switches, etc

firewall setting
	inbound traffic
		extensive filtering and firewall rules
		allow only required traffic
		config port forwding to map TCP/UDP ports to a devices 
		cnsider building a DMZ
	outbound traffic
	blacklist
	allow all, stop only unwanted traffic
	whitelist
	block all, only allow certain traffic types

disable ports
 	enable physical port
		conference rooms
		break room
	admin disable unused ports
		nore to maintain, but more secure
	network access control (nac)
		802.1x controls
		you can't communicate unless you are auth
content filtering
	control traffic based on data within the content
		data in the packets
	coporate control of outbound and inbound data
		sensitive materials
	control of inappropriate content
		not safe for work
		parental controls
	protection against evil 
		anti-virus, anti-malware
physical security 
	physical access - the easy part
	door access
		lock and key, electronic keyless
	biometric 
		eyeballs and fingers
	the process
		doc 
		well established