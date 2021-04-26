screen locks
	restrict access to the devices
		you're going to leave it somewhere
	fingerprint
	face unlock
	swip
	password
	failed attempts
		ios: erase everything after 10 failed attempts
		android: lock the devices and require a google login

anti-virus and anti-malware 
	apple ios 
		closed environment tightly regulated
		malware has to find a vuln
	android 
		more open, app can be installed from anywhere
		easier for malware to find it's way in
	app run in a "sandbox"
		you control what data an app can view

patching/OS update
	all devices need update
		even mobile devices
	device patches 
		security updates
	os update
		new features, bug fixes
	do not get behind
		avoid security problem

auth apps
	pseudo-random token gen 
		a useful auth factor
	carry around physical token devices
		where are my keys again
	you're carrying your phone around
		and it's pretty powerful

trusted vs. untrusted sources
	once malware is on a phone, it has a huge amount of access
		do not install APK files from an untrusted source
	ios 
		all app are curated by apple
	android 
		app can be downloaded from google play or sideloaded
		this is where the problem can occur

firewalls 
	mobile phones don't include a firewall
		mostt activity is outbound, not inbound
	some mobile firewall apps are available
		most for android
		none seem to be widely used
	enterprise environments can control mobile apps
		firewalls can allow or disallow access

policies and procedures
	manage company-owned and user-owned mobile devices
		BYOD - bring your own devices
	centralizrd management of mobile devices
		specialized functionality / Mobile Device Manager (MDM)
	set policies in apps, data, camera, etc
		control the remote device
		the entire devices or a "partition"