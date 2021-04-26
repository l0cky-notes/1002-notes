user and group
	user
		admin
			the windows super user
		guest 
			limited access
		standard users
	group 	
		power uses
			not much more control than a reqular users

NTFS vs share permissions
	NTFS permission apply from local and network connection
	share permissions only apply to connection	over the network\
		A "network Share"
	the most restrictive setting wins
		deny beats allow
	NTFS permissions are inherited from the parnet object
		unless you move to a different folder on the same volume

shared files and folders
	admin share
		hidden shares (i.e., C$) created during install
		local shares are created by users
	system files and folders
	 C$ -\
	 ADMIN$ - \ windows
	 PRINT$ - printers folder
	computer management / shared folder
		net share 

explicit and inherited permissions
	eplicit permissions
		set default permissions for a share
	inherited permissions
		propagated from the parnet object to the child object 
		set a permission once, it applies to everything underneath
	explicit permissions take precedence over inherited permissions
		even inherited deny permissions


run as admin
	admin have special rights and permissions
		edit sys files , install services
	use rights and permissions
		you don't get these by default even if you're in the admin group 
	right-click the app
		run as admin
		or ctrl-shift-enter
		
bitlocker
	encrypt an entire volume
		not just a single file
		protect all of your data, include the os
	lose your labtop?
		does not matter without the password
	data is always protected
		even if the physical drive is moved to another computer


EFS
	encrypting file system
		encrypr at the filesystem level
		on NTFS
	os support
		7,8,8.1, 10 pro enteprise
		7 ultimate
		10 education
	uses password and username to encrypt the key
		admin resets will cause efs files to be inaccessible