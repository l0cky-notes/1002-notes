the run line
	start an app as a command 
		termial based
	use the run/search or cmd
		specifty options as part of the command
	
cmd
	many options 
		the power under the hood

regedit
	the windows registry
		the big huge master database
		hierarchical structure
	used by almost everything
		kernal,device drives
		services 
		security account manager (SAM)
		user interface, app
	backup your registry
		built into regedit
services.msc
	control panel / admin tools / services
	useful when troubleshooting the startup process
	control background app
	serivces can reveal dep between app 
mmc
	microsoft management console
		build your own management framework
		choose from a list of "snap-ins"
	framework used for many built-ins management tools
notepad	
	a stupid text editor
	
msinfo32 
	windows system info
		A wealth of knowledge 
	hardware resources
		memory, DMA, IRQs, conflicts
	components
		multimedia, display, input, network
	software environment
		drives, print jobs, running tasks
	
dxdiag
	directx diagnostic tools
		manage your directx installation
	multimedia API
		3d graphices
		audio
		input options
	also make a very nice generic diagnostic tool
		not just for testing DirectX
	defrag
		disk defragmentation
			moves file fragment so they contiguous
			improves read and write trime
		not necessary for ssd
			windows won't defrag an SSD
		graphical version in drive properties
		requires elevation permissions
			command line:
				defrag <volume>
				defrag C:

system restore 
	create frequment restore points
		go back-in-time	to correct problems
	F8- advanced boot option- repair
	window 7/8/8.1/10:
	control panel/recovery
	doesn't guarantee recovery from viruses and spyware

windows update
	update system is automatic
	check for update but do not download to save bandwitch
	always check