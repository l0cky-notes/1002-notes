the password file
	different across os
		different hash methods
Brute Force 
	the password is the key 
		secret phrase
		stored hash
Brute Force Attacks
		keep trying the login
			very slow 
			most accounts will lockout after a number of failed attempts
		Brute Force the hash - offline
			obtain the list of users and hash
			calculate a password hash, compare it to a stored hash
			larger computational resource requirement
dictionary attacks
	people use common words as password
		you can find them in the dictionary
	if you're using brute force, you should start with the easy one
	many wordlists available on the ` net`
	this will catch the low-hanging fruit
rainbow tables
	an optimized, pre-built set of hashs
		doesn't need to contain every hash
		the calculations have been done
	remarkable speed increase
		especially with longer password
	need different table for different hashing methods
		windows is different than MySQL
	rainbow tables won't work with salted hashes
		add random value added to the original hash