RDP
	share a desktop from a remote location over TCP/3389
	remote desktop service on many windows version
	can connect to an entire desktop or just an app
	clients for windows, mac, linux,unix,iphone, and other



telnet
	tcp/23
	like ssh but unecrypted


ssh 
	tcp/22



third-party
	vnc (Virtual Network Computing)
		remote frame buffer (RFB) protocal
		clients for many os
		many are (FOSS)
	commercial solution
		teamviewe, logmeln, etc
	screen sharing
		control the desktop
	file sharing
		transfer files between devices




security considerations
	ms RDP
		an open port of tcp/3389 is a big tell
		brute force attack is common
	third-party remote desktop
		often secured with just a username and password
		there's a LOT of username/password re-use
	once you're in, you're in
		the desktop is all yours
		easy to jump to other system
		obtain personal information,  bank details 
		make purchases from the user browser