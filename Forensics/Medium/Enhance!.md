--------------------------------------------------------------------------------------------------------------
"
Download this image file and find the flag.
Download image file
"
--------------------------------------------------------------------------------------------------------------


wget "https://artifacts.picoctf.net/c/100/drawing.flag.svg"

# here we saw that the file is '.svg' that means it's XML-based 

cat darwing.flag.svg | grep -i "pico"

nano drawing.flag.svg

# here we see a lot of XMl and the flag is not visible 

# but if you read carefully you will see a weird text and characters like '{'

# so you need to take the text you have and remove all the useless text to have the flag (notepad++ will help)

>> picoCTF{3nh4nc3d_aab729dd}
