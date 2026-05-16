--------------------------------------------------------------------------------------------------------------
"
Can you crack the password to get the flag?
Download the password checker here and you'll need the encrypted flag in the same directory too.
"
--------------------------------------------------------------------------------------------------------------


wget "https://artifacts.picoctf.net/c/13/level2.py"

wget "https://artifacts.picoctf.net/c/13/level2.flag.txt.enc"

# you need to understand the code of the file to extract the password

cat level2.py

# the password is in '0x' (hex representation) in python 

python3

print(chr(0x64) + chr(0x65) + chr(0x37) + chr(0x36))

>> de76

python3 level2.py

de76

>> picoCTF{tr45h_51ng1ng_489dea9a}
