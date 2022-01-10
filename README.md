# simple hashing application - eVAHAN

To hash the 15-character driving license number of the format
		SS   CC   YYYY  NNNNNNN
Where,
	SS – State Code 
	CC – City Code
	YYYY- Year of Issue
	NNNNNNN – Actual license number

The program fetches the basic driver’s details just by using the hash value generated for that license number.
The license number is the value to which the key is to be hashed.
From 15-character license number only the last seven digits are taken to form the key.
For those digits (last 7 digits) division remainder hash function is used to generate the key for the hash table.


The idea of this function is to map a key k into one of the m slots by taking the remainder of k divided by m.
		h(k) = k mod m


Separate chaining technique is used for collision handling.
Open Hashing or separate chaining  is a collision avoidance method which uses array of linked list to resolve the collision. It is called as chaining because each linked list is considered as a chain.
