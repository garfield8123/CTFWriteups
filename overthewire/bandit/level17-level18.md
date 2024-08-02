# Level 18

Bandit OverTheWire Level 18: [level 18](https://overthewire.org/wargames/bandit/bandit18.html)

## **Level Goal**
There are 2 files in the homedirectory: passwords.old and passwords.new. The password for the next level is in passwords.new and is the only line that has been changed between passwords.old and passwords.new

NOTE: if you have solved this level and see ‘Byebye!’ when trying to log into bandit18, this is related to the next level, bandit19

## **Walkthrough**
- Figure out how diff works and order of diff files

## **level 18 Solution**
```shell 
diff passwords.old passwords.new
# last one because passwords.new
```

## **Generated password for level 18**
x2gLTTjFwMOhQ8oWNbMN362QKxfRqGlO
