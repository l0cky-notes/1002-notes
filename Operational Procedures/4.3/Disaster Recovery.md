backup strategies
	image level 
		bar metal backup using images
		os volume snapshot or hypervisor snapshop
		recover the entire system at once
		make an exact copy somewhere else
	file level
		copy individual files to a backup
		may not necessarily store all system files
		may need to rebuild the os and then perform a file restore




critical app backup 
	app software
		often distributed across multiple servers
	app data 
		databases, other data storage
	location of data
		local and cloud-based
	all of these are needed when restoring
		they all work together
	
	
	
	
backup testing
	it's not enough to perform the backup 
		you have to able to restore
	disaster recovery testing
		simulate a disaster situation
		restore from backup
	confirm the restoration
		test the restored app and data
	perform periodic audits
		always have a good backups




UPS
	uninterruptible power supply
		short-term backup power
		blackout, brown out, surges
	ups type
		offline/standby UPS
		line-interactive ups
		on/double-conversion ups
	features
		auto shutdown, battert cpacity, outlets, phone line suppression




surge suppressor
	not all power is "clean"
		self-inflicted power spikes and noise
		storms, power grid changes
	spikes are diverted to ground
	noise filters remove line noise
		decibel(db) level at a specified freq
			higher db is better
	

cloud storage
	data is available anywhere anytime on any devices
		if you have a network, you have your data
	advantages over local backups
		no tape drives to manage
		no offsite storage processing
	disadvantages over local backups
		data is not under your direct control
		strong encyption mechanisms are critical
		
		


account recovery options
	apps won't work if users can't login
		your windows domain will most likely be the foundation of your recovery files
	consider other auth requirments
		multi-factor auth valudation
		add auth databases
		RADIUS, TACACS
	another good reason for centralized admin
		no local account



equipment grounding
	most computer products connect to ground 
		divert any electrical faults away from people
	also applies to equipment racks
		large ground wire
	don't remove the ground connection
		it's there to protect you
	never connnect yourself to an elecrtrical ground
		this is not a way to prevent ESD





handling toxic waste
	batterices
		UPS
		dispose at your local hazardouse wast facility
	CRT's 
		cathode ray tubes - there's a few of those left
		class contains lead
		dispose at youre local hazardouse wast facility
	toner
		recycle and reuse
		many printer manaufactures provide a return box
		some office supply companies will provide  a discount for each cartridge




phone disposal
	wipe data
	manufacturer or phone serivce provide may have a recycling program
		or an upgrade program
	dispose at a local hazardous waste facility
		do not throw in the trash
		
		


personal safety
	remove jewelry
		and name badge neck straps
			or use breakaway lanyards
	safety lifting technique
	electricl fire safety
		DO NOT USE WATER OR FOAM
		use carbon dioxide, FM-200, or other dry chemicals
		rm the power source




personal safety
	cable management
		avoid trip hazards
		use zip tires or velcro
		make it look good
	safety goggles
		useful when working with chemicals
		printer repair, toner, batteries


goverment regulation
	health and safety laws
		vary widely depening on your location
		 keep the workplace hazard-free
		building code
			fire prevention, electrical codes
		environmental regulation
			high-tech waste disposal