--------------------------------------------------------------------------------------------------------------
"
Can you invoke help flags for a tool or binary? This program has extraordinarily helpful information...
"
--------------------------------------------------------------------------------------------------------------


wget "https://challenge-files.picoctf.net/c_wily_courier/5a478d0b24d6a4f4185e3adb7a78c41cdad626fb02fe80e083dc33bf8b197d3d/warm"

strings warm | grep "flag"

>> picoCTF{b1scu1ts_4nd_gr4vy_ac5832c}
