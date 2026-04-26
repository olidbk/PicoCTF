--------------------------------------------------------------------------------------------------------------
keygenme-py
--------------------------------------------------------------------------------------------------------------


wget "https://challenge-files.picoctf.net/c_wily_courier/26c4c19e611e4d55e34f14e4126af55fca948f10a675c1cab67bde103cca9282/keygenme-trial.py"

nano keygenme-trial.py

# first open it with "VSCode" to see the code better

# to know the variable "key_part_dynamic1_trial" regenerate it

---

import hashlib

flag = "picoCTF{1n_7h3_kk3y_of_"
bUsername_trial = b"BENNETT"

my_hash = hashlib.sha256(bUsername_trial).hexdigest()

nums = [4, 5, 3, 6, 2, 7, 1, 8]

key = ""

for num in nums:
    char = str(hashlib.sha256(bUsername_trial).hexdigest()[num])
    key += char

new_flag = flag + key + "}"

print(new_flag)

---

>> picoCTF{1n_7h3_kk3y_of_08c46aa4}

