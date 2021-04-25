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
smart cards
	must have physical card to provide digital access
		a digital cert 
	multiple factors
		card with pin or fingerprint
Anti-malware and anti-virus
	anti-malware software runs on the computer
		each device manages its own protection
	updates must be completed on all devices
		this becomes a scaling issue
	large organization need enterprise management
		track update, push updates, confirm update, manage engine update
network based firewall
	filters traffic by port number
		HTTP is 80, SSH is 22
		next-gen firewalls can identify the app
	can encrypt traffic into/out of the network 
		protecr your traffic between sites
	can proxy traffic 
		a common security techniqure
	most firewall can be layer 3 devices (router)
		usually sits on the ingress/egress of the network
user auth 
	identifer
		something unique
		in windows, every account has security id (SID)
	cred 
		the info used to authenticate the user
		password, smart card, PIN code, etc
	profile
		information stored about the user
		name contact info, group memberships, etc
strong password
	weak password can be difficult to protect agaunsy
	 brute force
	 brute force the hash
passwords need to complexity and constant refresh
	reduce the change of a brute force 
	reduce the scope if a password is found
anual password analysis from splash data
	examines leaked passsword files

multi-factor auth 
	more than on factor
		something you are
		something you have
		something you know
		somewhere you are
		something you do
	can be expensive
		separate hardware tokens
	can be inexpensive
		free smartphone app software-based token generator
directory permissions
	ntfs permissions
		much more granular than FAT
		lock down access
		prevent accidental modification or deletion
		some info shouldn't be seen
	user permission
		evertone is not admion
		assign proper right and permission
		this may be an involved audit
vpn concentrator
	virtual private network 
		encrypt data traversing a public network 
 	concentrator
 		encryption/decryption access devices
	many deployment options
		specialized cryptographic hardware
		software-based option	available
Data loss prevention (DLP)	
	where is your data?
		ssn, credit card number, medical records
	stop the data before the bad guys get it
		data 'leakage'
	so many sources, so many destination
		often requires multiple solutions in different places
access control lists (ACLs)
	used to allow or deny traffic
		also used for NAT, QoS, etc.
	defined on the ingress or egress of an interface
		often on a router or switch
		incoming or outgoing 
	ACLs evalute on certain criteria
		source IP, Destination IP, port number, ICMP
	deny or permit
		what happens when an ACL match the traffic?
		
email filtering
	unsolicited email 
		stop it at the gatway before it reaches the users
		on-site or cloud-based
	scan and block malicious software
		exec, know vulnerabilites
		phishing attempts
		other unwanted content
trusted/untrusted software sources 
	conider the source
		may not have access to the code
		even then, may not have the time to audit
  trusted soucre
  	internal app
	well-know publishers
	digitally-signed app
	untrusted sources
		app from third-party sites
		links from an email pop-up/ drive by downloads
least privilege 
	right and permission should be set to the bare mini
		you only get exactly what's needed to complete your objective
all user accounts must be limited 
	app should run with a minimal privilges
don't allow users to run admin privileges
	limited the scope of malicaious behavior