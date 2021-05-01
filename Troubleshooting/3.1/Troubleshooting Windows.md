slow system preformance
	task manager 
		check for high CPU utilization and I/0
	windows update
		latest patch and drives
	disk space
		check for available space and defrag
	laptops may be using power-saving mode
		throttles the cpu
	anit virus and anti malware

limited connectivity
	limited or no connect: the connect has limited or no commectivity. you might be unable to access the Internet or some network resources. the connection is limited
	local issues
		wireless  signal, disconnected cable
		check ip address config
		reboot
	external issues
		wireless router rebooted/turned off
		ping your default gateway and external ip

boot error 
	can not find the os
		os missing
	boot loader replaced or changed 
		multiple os installed 
	check boot drives
		remove any media
	startup repair
	modtify the windows boot configuration database (BCD)
		formerly boot.init
		recovery console bootrec / rebuild bcd
	
startup repair
	missing NTLDER
		the main windows boot loader is missing
			run startup repair or replace manually and reboot 
			disconnect removable media
	missing os
		boot configuration data may be incorrect
		run startup repair or manually configure BCD store
	boots to safe mode
		windows is not starting normally
		run startup repair

app crashes
	app stop working
		may provide an error message
		may just disappear
	check the event log
		often includes useful reconnaissance
	check the reloability monitor 
		a history of app problems
		check for resolutions

bluescreen and spotaneous shutdown 
	startup and shutdown BSOD
		bad hardware , bad drivers, bad app
	use last know good, system restore or rollback driver
		try safe mode
	reseat or remove the hardware
		if possible
	run hardware diagnostics
		provided by the manufacturer
		BOIS may have  hardware diagnostics
	
black screen 
	no login dialog, no desktop 
		driver corruption os file corruption
	start in VGA mode
		f8 for startup options
	run SFC
		system file checker
		run from recovery console
	update driver in safe mode
		download from known good sources
	
test printer 
	print or scan a test page 
		built into windows 
		not the app
	use diagnostic tools
		web-based utilites
			built into the printer
		vendor specific
			download from the web site
		generic
			available in LiveCD form
	
starting the system 
	device not starting 
		check device manager and event viewer
		often bad drivers
		1:remove or replace drivers
	"one or more services failed to start"
		bad/incorrect driver, bad hardware 
		1:try starting manually
		2:check account permissions
		3:confirm service; dependencies
		4:windows services; check system files
		5:application services; reinstall app
		
slow boot 
	boot process hangs or takes longer than normal 
		no activity, no drive lights
	manage the startup apps
		control what loads during boot process
	task manager
		startup tab
		startup impact, right-click / disable

slow profile load 
	roaming user profile
		your desktop follows you to any computer
		changes are synchronized
	network latency to the domain controller 
		slow login script transfer
		slow to apply computer and user policies
		may require many hundreds (or thousands) of LDAP queries
	client workstations picks a remote domain controller instead of local dc
		problems with local infrastructure