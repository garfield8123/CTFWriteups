## **Common Commands**

### **Common Username/password**
- Username: root, admin, sysadmin, user, test
- Password: password, password123, password1234, 1234

### **Nmap**
```bash
nmap -v -A <ip-address> -p <port-range>
```
![nmap_Cheat_sheet](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fsecurityonline.info%2Fwp-content%2Fuploads%2F2017%2F08%2Fnmap.png&f=1&nofb=1&ipt=5ab6028ec932ef96018cb00657dc4100175e4674b98cb998b3cfc36e89bdeff5&ipo=images)

### **Content Discovery**
```bash
curl <site>/sites/favicon/images/favicon.ico | md5sum

gobuster dir --url <site> -w <wordlist>
```
[MD5_Favicon_Database](https://wiki.owasp.org/index.php/OWASP_favicon_database)
[Web_Framework_analyzer](https://www.wappalyzer.com/)

### **Brute Force Login**
```bash
crunch <min> <max> <characters> -o <output.txt>

# uses the login field as "" empty string and uses the passwords teh 3digits.txt until it finds a working password with the finds the http method being used pin code is submitted to login.php:pin=^PASS^ allows the passwords from 3digts.txt to be inputed then it looks for the string Access denied when the password fails and the port is 8000
hydra -l '' -P 3digits.txt -f -v MACHINE_IP http-post-form "/login.php:pin=^PASS^:Access denied" -s 8000
```
[Hydra Cheatsheet](https://github.com/frizb/Hydra-Cheatsheet)
