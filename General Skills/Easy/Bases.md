# Bases Writeup

> What does this bDNhcm5fdGgzX3IwcDM1 mean? I think it has something to do with bases.

## Solution

**you can use cyberchef to make it easy. but you can use terminal too.
let's try base64 because it's the most famous one**

```shell
echo "bDNhcm5fdGgzX3IwcDM1" | base64 -d
```

```text
l3arn_th3_r0p35
```

```flag
picoCTF{l3arn_th3_r0p35}
```

