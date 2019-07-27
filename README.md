# Secrypt

## Simple Crypting library for python

Usage:

```python
import secrypt

# create a crypt object
c = secrypt.Crypt(key=0.0)	# key : 0.0 is the default

# encrypt string
data = "hello world!"
en = c.encrypt(data)	# returns encrypted data

# decrypt string
de = c.decrypt(en)		# returns original data

# write encrypted file
content = """Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
proident, sunt in culpa qui officia deserunt mollit anim id est laborum."""

c.write("test.txt", content)	# returns size of encrypted file

# read encrypted file
retrieved = c.read("test.txt")	# return original file data

```
