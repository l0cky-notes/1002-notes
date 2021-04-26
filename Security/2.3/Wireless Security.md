wireless encryption
	all wireless computer are radio transmitters and receivers
		anyone can listen in
	anwser: encrypt the data
		everyone gets the password
		or their own password
	only people with the password can transmit and listen
		wpa and wpa2
	
wpa 
	2002: wpa was the replacement for wep DO NOT USE WEP 
   needed a short-term bridge between WEP and whatever would be the successor
   	run on existing hardware
 wpa: RC4 with TKIP(Temporal  Key Integrity Protocal)
 	initalization vector (IV) is larger and an encrypted hash
	every packet gets a unique 128-kit encryption key


Temporal  Key Integrity Protocal
	mixed the key 
		combines the secret root key with the IV
	adds a sequence counter
		prevents replay attacks 
	implements a 64-bit message integrity check
		protects against tampering
	TKIP has it's own set of vulnerabilitys
		deprecated in the 802.11-2012 standard

wpa2 and ccmp 
	wpa2 certification began in 2004
		aes (Advanced_Encryption_Standard) replaced RC4
		ccmp(Counter Mode Cipher Block Chaining Message Authentication Code Protocol) replaced TKIP
	ccmp block cipher mode
		uses AES for data confidentiality
		128-bit key and a 128-bit block size
		requires add computer resources

wireless security modes
	config the auth on your wap/ wireless router
	open system
		no password is required
	wpa2-personal/wpa2-psk
		wpa2 with a pre-shared key
		everyone uses the same 256-bit key
	wpa2-enterprise/wpa2-802.1x
		auth user individually with auth server (i.e., RADIUS, TACACS+)
		add additional factors

RADIUS (Remote Authentication Dial-In User Service)
	one of the common AAA protocal
		support on a wide variety of platform and devices
		not just for dial-in
	centralize auth for users
		router, switches, firewall
		server auth
		remote VPN access
		802.1x network access
	RADIUS services available on almost any server os


TACACS (Terminal Access Controller Access-Control System)
	Terminal Access Controller Access-Control System
		remote auth protocol
		created to control access to dial-up lines to ARPANET
	TACACS +
		the latest version of TACACS
		more auth requests and response code
		released as an open standard in 1993