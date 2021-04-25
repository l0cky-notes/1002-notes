Active Directory
	centralized management
		windows domain services
		limit and control access
	login scripts
		map network drives
		update security software 
		update app software
	group policy  / update 
		define specific policies
		password complexity
		login restrictions
	organiztional units
		structure active directory
		can be based on the company (location,deparment)
	home folder
		assign a network share as the user's home
		\\server1\users\liam
	folder redirection
		instead of a local folder, redirect to the server 
		store doc folder \\server1
		access file from anywhere
	
mobile devices management (MDM)
	manage company-owned and user-owned mobile devices
		BYOD - bring your own devices
	centralized management of the mobile devices
		specializedf functionality
	ser policies on app,data,camera, etc
		control the remote devices
		the entire devices or a "partition"
	manage access control 
		force screen locks and pins on these single users devices

port scrurity
	prevent unauthorized users from connecting to a switch interface
		alert or disable a port
	based on the source MAC address
		even if forwarded from elsewhere
	each port has it own config
		unique rules for every interface

port security example 
	config a max number of sorce MAC address on an interface
		you decide how many is too many
		you can also confgure specifi MAC address
	