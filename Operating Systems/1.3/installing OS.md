boot methods
	usb storage
		usb must be bootable 
		computer must support booting from USB
	CD-ROM and DVD-ROM
		a common media
	PXE ("Pixie") - preboot eXecution Environment
		preform a remote network installation
		computer must support booting with PXE
	NetBoot
		Apple tech to boot macOS from the network
		similar concept to PXE

ssd/hard drive
		store many OS installation files
	external/hot swappable drive
		some external drive can mount a ISO
		boot USB
	internal hard drive
		install and boot from separate drive
		create and boot from new partition
	
	
type of installation
	ubattended installation
		answer windows question in a file(unattend.xml)
		no installion iterruption
	inplace upgrade
		maintain existing app and data
	clean install
		wipe the slate clean and reinstall
		migration tool can help
	image 
		deploy an clone on every computer
	repair installation
		fix problem with the windows OS
		does not modify user files
	multiboot 
		run two or more operation systems from a single pc
	recovery partition
		hidden partition with installation files
			refresh/restore
		windows 8/10 feature to clean things up
		requires a recovery patiton
		
	
the disk partion
	sep the physical drive inot logical pieces
		useful to keep data separated
		multiple patitions are not always necessary
	useful for maintaining separate operating system
		windows,linux,etc
	formatted patitions are called volumes
		microsoft's nomenclature
		
MBR patition style
	MBR (Master Boot Record)
		the old standby, with all of the old limitations
	primary
		bootable partitions
		max of four primary patitions per hard disk
		one of the primary patitions can be marked as Active
	extended
		used for extending the max number of partions
		one extended partition pre hard disk (optional)
		contains add logical partition per hard disk (optional)
		contains add logical partitions
		logical patitions inside an extended patition are not bootable
		

GPT partition style
	GPT(GUID partition table)
		globally unique identifer
		the latest patition format standard
	requires a UEFI BIOS
		can have up to 128 partitions
	no need for extended partitions or logical drive
	
disk patitioning
	the first step when preparing disks
		may already be partitioned
			existing partitions may not always be compatible with your new operating system
	
an MBR-style hard disk can have up to four partitions
	 GUID patition table support up to 128 patitions
		requires UEFI BIOS or BIOS-compatibility mode
		BIOS-compatibility mode disables UEFI secureBoot
	be careful
		serious potential for data loss
		this is not an everyday occurrence
		
		
storage types
	layered on top of the partition and file system
		a windows thing
	basic disk storage
		available in DOS and windows versions
		primary/extended patitions, logical drives
		basic disk partitions can't span separate physical disks
	dynamic disk storage
		available in all modern windows version
		span multiple disks to create a large volume 
		split data across physical disks (striping)
		dup data across disk (mirroring)
			not all wind version support all cap
			

file systems
	before data can be written to the partitions, it must be formatted
		build the foundation\
	os expect data to be written in paticular format 
		FAT32 and NTFS is pop
	many os can read (and perhaps write ) multiple file system types
		FAT,FAT32,NTFS,exFAT,etc.
	

FAT 
	FAT-file allocation table 
		one of th efirst PC-based file system
	FAT32-file allocation table
		larger(2 terabyte) volume sizes
		max files size of 4 gb
	extFAT- Extended file allocation table
		microsoft flash drive file system
		files can be larger than 4 giga
	
NTFS and CDFS
	NTFS - NT file system
		extensive improvements over FAT32
		quotes, file compresssion, encryption, symbolic links, large file support, security, recoverability
	CDFS - Compact Disk File System
		ISO 9660 standard
		all operating system can read the CD
		
other file system 
	ext3 
		third extended file system
		commonly used by the linux OS
	ext4 
		fourth extended file system
		an update to ext3
		commonly seen in linux and android 
	NFS
		Network file system
		access files across the network as if they were local
		NFS clients available across many operating system
	HFS+ / HFS plus
		hierarchical file system
		also called mac os extended
		replaced by apple file system
		(APFS) in macOS High Sierra
	swap partion
		memory management 
		frees memory by moving unused pages onto disk 
		copies back RAM when needed
		usually a fast drive or SSD
		
quick format vs full format 
	quick format
		create a new file table
			looks like data is erased, but it's not 
		no add check
	quick format in windows 7,8 and 10
		use DISKPART for full format 
	full format 
		writes zeros to the whole disk
			your data is unrecoverable
		checks the disk for bad sectors - time consuming
		
other consideration
	load alternate third party drive when necessary 
		disk controller drivers, etc
	workgroup vs domain setup
		home vs business
	time/date/region/lang settings
		where are you?
	driver installation, software and windows updates
		load drivers,install apps, update the os
	factory recovery partion
		this can help you later