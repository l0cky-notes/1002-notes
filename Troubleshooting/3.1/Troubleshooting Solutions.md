defragmentation
	moves file fragment so they are contiguous
		sharing a common border
		improves read and write time
		only app to spinning hard drive
	gui in the drive properties
		command line defrag
	weekly schedule
		use control pannel / admin tools / task scheduler

kill tasks
	instead of rebooting find the problem
		and kill it
	task manager 
		processes tab
	sort by resource
		cpu, memory, disk, network
	right-click to end task
		trial and error


update network settings
	one configuration mismatch can cause significant network slowdowns
		speed
		duplex
	most auto negotiations work fine
		until they do not
	driver may not show the negotiated value
		filter through the event viewer
	device should match the switch
		both sides should be id

reimage or reload OS
	windows is big
		and complex 
	spend time trying to find the needle
		or build a new haystack
	many organizations have prebuilt images
		do not waste time researching issues
	windows 8/8.1 and 10 includes a reset options
		setting  / update & security / recovery


roll back 
	restore points
		rewind to an earlier point in time
		time travel without erasing your work
	app updates
		restore created auto during appp installations
	device drivers
		these can break windows 
		roll back from the windows start menu (F8)
		
update and patch
	windows update
		centralized OS and drive update
	lots of flexibility
		change active hours
		manage metered connections
	app must be patched
		security issues don't stop at the os
		download from the publisher


update boot order
	try to boot fromt a USB drive
		doesn't even try
	the bios detemines which physical devices will be used during boot
		and in which order
	each bios is a bit different
		the config is in there somewhere
	it's an easy one to miss
		usually the first thing to check

disable startup services / apps
	it's difficult to tell what app might be a problem child 
			much of the underlying os operations are hidden from view
	trial and error 
		disable all startup apps and serivices
		or disable one at a time
		this might take quite a few restarts
	manage startup processes 
		task manager or conrol panel / admin tools / sevices

safe mod - windows 7 and 8/8.1
	press f8 on boot 
		advanced boot options
	safe mode 
		only the necessary drivers to get started
	safe mode with networking
		include drivers for network connectivity
	safe mode with command prompt
		no windows explorer - quick and dirty
	enable low-resolution (VGA mode)
		recover from bad video driver installations

safe mode - windows 10
	f8 probaly won't work
		windows fast setup in windows 8/8.1 and windows 10 prevents a complete shutdown
	from the windows desktop
		hold down shift when clicking restart 
		settijng / update & security / recovery / advanced startup / restart now
		system configuration (msconfig)
	interrupt normal boot three times
		presents the boot options screen
	
	
	
rebuild windows profile
		profiles can become corrupted
			the user profile service failed the logon. user profile con not be loaded
			user documents may be "missing"
		if a profile doesn't exist, it is recreated
			we're going to delete the profile and force the rebuilding process

deleting windows profiles
	login to the computer with domian admin rights
	rename the \User\name folder
		this will save importantt files
	backup the user's registry
		HKLM\SOFTWARE\Mircosoft\Windows NT\CurrentVersion\ProfileList
		right-click /export
	delete the registry entry
			you have a backup 
	restart the pc



reconstructing windows profile
	login to the computer witrh the user account 
		the profile will rebuilt
		this will recreate the \User\name folder
	login as Domain Admin
		copy over any important files from the old profile
	do not copy the entire profile
		corrupted files might exist in the old profile
	logout as domain admin, login with the user account