--------------------------------------------------------------------------------------------------------------
"
Can you crack the password to get the flag?
Download the password checker here and you'll need the encrypted flag in the same directory too.
"
--------------------------------------------------------------------------------------------------------------


wget "https://artifacts.picoctf.net/c/11/level1.py"

wget "https://artifacts.picoctf.net/c/11/level1.flag.txt.enc"

# first you need to read the code and understand it 

cat level1.py

python level1.py

# he will ask you for a password so in the source code the password is "1e1a"

1e1a

>> picoCTF{545h_r1ng1ng_fa343060}
