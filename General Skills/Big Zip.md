--------------------------------------------------------------------------------------------------------------
"
Unzip this archive and find the flag.
Download zip file
"
--------------------------------------------------------------------------------------------------------------


wget "https://artifacts.picoctf.net/c/505/big-zip-files.zip"

unzip big-zip-files.zip/

# here we saw a lot of files and directories so the best command is "grep"

grep -ri "picoctf" big-zip-files/
