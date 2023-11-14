# Hashcat Examples

```
# SHA512crypt $6$ shadow file  
hashcat -m 1800 -a 0 -O -w 4 hash rockyou.txt

# MD5 $1$ shadow file  
hashcat -m 500 -a 0 -O -w 4 hash rockyou.txt

# MD5 Apache webdav file  
hashcat -m 1600 -a 0 -O -w 4 hash rockyou.txt

# SHA1
hashcat -m 100 -a 0 -O -w 4 hash rockyou.txt 

# SHA2
hashcat -m 1400 -a 0 -O -w 4 hash rockyou.txt 

# Wordpress  
hashcat -m 400 -a 0 -O -w 4 hash rockyou.txt 

# NTLM
hashcat -m 1000 -a 0 -O -w 4 hash rockyou.txt

# SHA256crypt
hashcat -m 7400 -a 0 -O -w 4 hash rockyou.txt

# md5
hashcat -m 0 -a 0 -O -w 4 hash rockyou.txt

# SHA2-224
hashcat -m 1300 -a 0 -O -w 4 hash rockyou.txt

# NetNTLMv2
hashcat -m 5600 -a 0 -O -w 4 hash rockyou.txt

# Kerberos 5, etype 23, AS-REP
hashcat -m 18200 -a 0 -O -w 4 hash rockyou.txt

# Kerberos 5, etype 23, TGS-REP
hashcat -m 13100 -a 0 -O -w 4 hash rockyou.txt
```

url="https://hashcat.net/wiki/doku.php?id=example_hashes"