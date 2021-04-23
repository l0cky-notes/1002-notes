privileges 
	not all users can run all commands
		some ifno and task are for root users only
	stanadard privileges
		run app as normal user
		this works fine for many command
	admin / root privileges
		you must be a member of the admin group 
		right-click cmd, choose run as admin
		cmd,ctrl + shift + enter
		
cmd troubleshooting 
	use "help" if not sure
		help dir
		help chkdsk
	also use
		[command] /?
	close the prompt with exit

shutdown
	shutdown a pc 
		and optionally restart
	shutdown /s /t nn
		wait nn seconds, then shutdown
	shutdown /r /t nn
		shutdown  and restart after nn seconds
	shutdown /a 
		abnort the countdown!
	
dism
	deployment image servicing and management tool
		manage windows imaging format (WIM) files
	make change to your image with DISM
		get info about an image 
		update app
		manage drivers 
		manage updates
		mount an image
sfc 
	system file checker
		scan integrity of all protected system files

check disk
	chkdisk /f
		fixes logical file system error on the disk
	chkdsk /r
		locales bad sectors and recovers readable information
		implies /f
	if volume is locked run during startup
	
managing group policy
	group policy
		manage computer in an active directory domain
		group policy is usually update at login
	gpupdate
		force a group policy update
		gpudate /target:{computer | user} /force
		gpupdate /target: liam /force
		
	gpresult
		verify policy settings for a computer or user
			gpresult /r
			gpresult /user sge /liam /v
format
	formats a disk for use with windows 
		be carful - you can lose data 

copy (/v, /y)
	/v - verifies that new files are written correctly 
	/y suppresses prompting to confirm you want to overwrite an existing destination file
	
	
xcopy 
	copies files and directory trees 