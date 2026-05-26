--------------------------------------------------------------------------------------------------------------
"
Can you crack the password to get the flag?
Download the password checker here and you'll need the encrypted flag and the hash in the same directory too. 
Here's a dictionary with all possible passwords based on the password conventions we've seen so far.
"
--------------------------------------------------------------------------------------------------------------


wget "https://artifacts.picoctf.net/c/31/level5.py"

wget "https://artifacts.picoctf.net/c/31/level5.flag.txt.enc"

wget "https://artifacts.picoctf.net/c/31/level5.hash.bin"

wget "https://artifacts.picoctf.net/c/31/dictionary.txt"

# here they give you a file of passwords, so first you need to know how to loop through a file in python

cat level5.py

# so here i add new lines of code, that makes you try all the passwords in the file

nano my_level5.py

# and i add my code befor level_3_pw_check() function 

---

with open("dictionary.txt", "r") as file:
    for pw in file:
        my_hash = hash_pw(pw.strip())
        if my_hash == correct_pw_hash:
            print(pw.strip())

---

python3 my_level5.py

>> 9581
>> Please enter correct password for flag:

9581

>> picoCTF{fl45h_5pr1ng1ng_cf341ff1}
