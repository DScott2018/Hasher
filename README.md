This repository contains a Hash function written in Python. The function uses the 'hashlib' module as this module already contains popular hashing algorithms such as sha256, md5, sha1, etc.

When running this script, you will be asked to input data to be hashed and the algorithm you wish to use to hash the data. If the algorithm is not recognized by the hashlib module, it will default to sha256.

noSalt will output data hashed without a salt, meaning this data could be vulnerable to a rainbow table. For demonstration purposes, this script has been included to show the difference between salted and un-salted hashes.

Salted will output the data hashed with a salt. This hash will be much more difficult to determine the original data. Rainbow tables should not work against this type of hash function.
The salt can be input within the parameters of the method or left as 'None'. If it is left as none, then the 'os' module will generate a random 16 bit salt to be appended to the end of the data to be hashed.
