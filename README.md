# Venom
###### This script takes domain name, working directory path, altdns.txt, huge list of DNS resolver and a list of Google DNS servers 8.8.8.8 & 8.8.4.4. And You get the output in the working directory as Aquatone Screenshots, a subdomains.lst list of subdomains found, a ip.lst list of IP addresses and Masscan XML
## Prerequisites:
### Tools in Path variable of your Linux:
##### amass
##### sublist3r
##### massdns
##### altdns
##### aquatone
##### Subfinder

### Files from this repository:
##### Venom.sh
##### resolvers.txt (This is a list of resolvers, you are free to use your own)
##### resolve-verify.txt
##### altdns.txt

## Usage:
###### The first argument is domain_name
###### The second argument is working_directory.
###### The third argument is DNS resolvers list placed in file "resolvers.txt"
###### The fourth argument is list of two Google DNS resolvers for last verification of subdomains is done by using Google Dns servers 8.8.8.8 & 8.8.4.4
###### The fifth argument is AltDNS wordlist called altdns.txt from this repository.
```
cd /root/tools/venom/

bash venom.sh example.com /root/example /root/tools/venom/resolvers.txt /root/tools/venom/resolve-verify.txt /root/tools/venom/altdns.txt
```



# Output:
#### subdomains.lst -- All subdomains
#### masscan.xml -- Masscan output in XML
#### aquatone/ip -- Aquatone screenshots of IP addresses
#### aquatone/subs -- Aquatone screenshots of subdomains.lst
#### amass.lst -- Raw list by Amass
#### subfinder.lst -- Raw list by Subfinder
#### sublist3r.lst -- Raw list by Sublist3r
