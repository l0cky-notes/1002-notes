password complexity an length	
	make your password strong 
		no single word
		do not be obvious
			what's the name of your dog
		mix upper and lower case
		use special characters
			don't replace o with 0 or t with 7
	a strong password is at least 8 characters
		consider a phrase or set of words
	set password expiration, require change
		sys remembers password history, requires unique passwords\

desktop security
	require a screensaver password
		integrate with login cred
		can be admin enforced
		auto lock after timeout
	disable autorun
		autorun.inf in Vista
			no autorun in windows 7,8/8.1, or 10
		disable through the registry
	consider changing autoplay
		get the lastest security patches
			update to autorun.inf and autoplay

password best pratices
	changing the default
		all device have default
		there are many stites witr doc these	
	bois/UEFI passwords
		supervisor/admin password: prevent BIOS changes
		user password: prevent booting
	requiring password
		always require password
		no blank password
		no auto login
restricting user permissions
	user permissions
		everyone is not an admin
		assign proper rights and permissions
		this may be an involved audit
	assign rights based on groups
		more difficult to manage per-user rights
		become more useful as you grow
	login time restrictions
		only login during work hours
		restrict after-hours acticities


account lockout and disablement
	too many bad password will cause a lockout
		this should be normal for most users
		this can cause big issues for service accounts
			you might want this
	disable users account 
		part of the normal change process
		you don't want to delete accounts
			at least not initially

data encryption
	full-disk encryption
		encrypt everything
	filesystem encryption
		individual files and folders
	protect those usb flash drive
	key backups are critical
		you always need to have a copy
		this may be integrated into AD
		you'll want to keep the key handy

patches and update management
	keep OS and app updated
		security and stability improvements
	built-in to the os
		updates are deployed as availale
		deployment may be managed internally
	many app include their own updater
		check for updates when starting
	always stay up to date
		security vuln are exploited quickly