scheduled backups
	many options
		cmd and gui
		may be include with the ditro
	tar
		tape archive
		easy to script into a backup schedules
	rsync
		sync files between storage devices
		instant synch or scheduled
	
scheduled disk maintenance
	very litte disk maintence required
		space and resources
	check file system
		files system can't be mounted
		done automatically every X number of reboot
		force after reboot by adding a file to the root
			sudo touch /forcefsck
		clean up log space
			/var/log
		system update
			command line tools
				apt/apt-get, yum, pacman
			gui update manager
				software updater
			patch management
				updates can be scheduled
			software center
				the linux "app store"
driver/firmware updates
	many drivers are in the kernel
		updated when the kernal updates
	add drivers  are managed with software update or at the command line
		update those yourself
	anti-virus/anti-malware update 
		relatively few viruses and malware for linux
			UPDATE
		clamAV
			OPEN SOURCE antivirus
		same best practice as any other OS
			always update signature database
			always use real-time scanning
	