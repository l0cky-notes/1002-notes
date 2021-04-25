[youtube](https://www.youtube.com/watch?v=tG6JfLepOP8&list=PLG49S3nxzAnmwkCAdWUgCFvVK4IxMBTmb&index=30)
linux command 
	the command line 
		terminal, Xterm, or similar
	command are similar in both linux and macOS 
		macos derived from BSD unix
		this video is specific to linux
	download a live CD or install a vm
		many pre-made linux distro are available 
		I'm using Ubuntu in a virtual machine
	use the man commad for help
		man grep
ls 
	list directory contents
		similar to the dir connad in windows
	list files, directories
	 may support color coding; 
	 blue is a directory
	 red is an archive file, etc
	for long output, pipe through more:
		[[ls -l | more (use q or Ctrl-c to exit ]]
	[[	commads]]

shutdown 
	shut down the system
sudo shutdown 2
	shuts down and turns off the computer in 2 miin	
sudo shutdown -r 2 
	important when you're not on site
ctrl-c or shutdown -c
	to canel
pwd vs. passwd

pwd 
	print working directory
	displays the current working directory path
	useful when changing directories often
	useful to when changing directories often


paswd
	change passwd
	passwd [username ]


mv 
	to move/rename a file
	mv first.txt second.txt


rm
	remove a file or directories
		delete the file
	does not remove a director by default
		dir must be empty to be removed
		or must be removed with -r


chmod
	change mode of a file system object
		r=read, w=write, x=execute
		can also use octal notation
		set for file owner (u), group(g), other(o), or all(a)
		![[Pasted image 20210424142940.png]]
		chmod 744 first.txt 
			user; read, write exec
			group, read only
			other; read only
		chmod a-w first.txt
			all user, no writing first.txt
		chmod u+x script.sh
			the owner of script.sh can exec file


chown 
		change file owner and group 
			modify file setting
		sudo chown [OWNER:GROUP] file
			sudo chown liam script.sh
		
iwconfg/ifconfig
	iwconfig 
		view or change wireless network config
		essid, freq/channel, mode, rate,etc
		requires some knowledge of the wireless network
		iwconfig wlp4s0 essid Terrytown
	ifconfig
		view or config a network interface and IP config
		ifconfig eth0
		slowly being replaced by ip(ip address)
		
ps
	view the current processes
		and the process id (pid)
		similar to the windows task manager
	view user processes
		ps
	view all processes
		ps -e | more
vi
	text editor
dd
	dd if=source file name of= target file name [options]
