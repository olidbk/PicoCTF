--------------------------------------------------------------------------------------------------------------
Can you find the flag in file without running it?
--------------------------------------------------------------------------------------------------------------


wget "https://challenge-files.picoctf.net/c_fickle_tempest/094a1db42d5ae681cd9e513dcbea2d997495dd3763d50c643b939923ca86e29b/strings"

strings strings | grep "pico"

>> picoCTF{5tRIng5_1T_47948C73}
