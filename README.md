# dnsbash
Just a small DNS bruteforcer written in bash.

### Usage
```
./dnsbash <domain> [wordlist]
```

The wordlist is optional. When none is provided dnsbash uses the provider example wordlist. If you need a good wordlist checkout [https://github.com/danielmiessler/SecLists/tree/master/Discovery/DNS](https://github.com/danielmiessler/SecLists/tree/master/Discovery/DNS).

### Example
```
[yoram]#[~] _  dnsbash kali.org ./wordlist.example
> dnsbasher

  [+] dnsbashing kali.org
  [+] Using wordlist: ./wordlist.example
  [+] Wordlist contains 11 lines.

git.kali.org.		59	IN	CNAME	hephaestus.kali.org.
hephaestus.kali.org.	59	IN	A	67.23.72.103
mail.kali.org.		59	IN	CNAME	apollo.kali.org.
apollo.kali.org.	59	IN	A	23.239.31.82

Performed 19 queries in 1 seconds.

Done
```
