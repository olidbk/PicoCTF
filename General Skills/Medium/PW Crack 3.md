--------------------------------------------------------------------------------------------------------------
"
Can you crack the password to get the flag?
Download the password checker here and you'll need the encrypted flag and the hash in the same directory too.
There are 7 potential passwords with 1 being correct. 
You can find these by examining the password checker script.
"
--------------------------------------------------------------------------------------------------------------


wget "https://artifacts.picoctf.net/c/18/level3.py"

wget "https://artifacts.picoctf.net/c/18/level3.flag.txt.enc"

wget "https://artifacts.picoctf.net/c/18/level3.hash.bin"

nano level3.py

# in the code they give us a list of the possible passwords

# so here i add new lines of code, that makes you try all the passwords in the list

nano my_level3.py

# and i add my code befor level_3_pw_check() function 

---

pos_pw_list = ["8799", "d3ab", "1ea2", "acaf", "2295", "a9de", "6f3d"]
for pw in pos_pw_list:
    my_hash = hash_pw(pw)
    if my_hash == correct_pw_hash:
        print(pw)

---

python3 my_level3.py

>> 2295
>> Please enter correct password for flag:

2295

>> picoCTF{m45h_fl1ng1ng_6f98a49f}
