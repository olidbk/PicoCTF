# Big Zip Writeup

> Unzip this archive and find the flag.
> [Download zip file](https://artifacts.picoctf.net/c/505/big-zip-files.zip)

## Solution

```shell
wget "https://artifacts.picoctf.net/c/505/big-zip-files.zip"
```

```shell
unzip big-zip-files.zip/
```

**here we see a lot of files and directories so the best command here is 'grep'**

```shell
grep -ri "picoctf" big-zip-files/
```

```flag
picoCTF{gr3p_15_m4g1c_ef8790dc}
```

