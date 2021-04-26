Spoofing
	pretend to be something you aren't
		fake web server,fake DNS server, etc
	email spoofing
		the send addr of an email isn't really the sender
	caller id spoofing
		the incoming call info is completely fake
	man-in-the-middle attack
		the person in the middle if the conversation pretends to be both endpoints
MAC spoofing
	ethernet devices has a mac addr
		a unique burned-in address
		most drivers allow you to change this
	changing the MAC addr can be legitimate
		internet provider expects a certain MAC addr
		certain app require a particular mac addr
	it might not be legitimate
		circumvent MAC-based ACL's
		fake-out a wireless address filter
	very difficult to detect
ip addr spoofing
	take someone else's ip addr
		actual device
		pretend to be somewhere you are not
	can be legitimate
		load balancing
		load testing
	may not be
		ARP poisoning
		DNS amplification / DDoS
	easier to identify than MAC address spoofing
		apply rules to prevent invalid traffic, enable switch security