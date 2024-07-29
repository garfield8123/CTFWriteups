# Level 0

Bandit OverTheWire Level 0: [level 0](https://overthewire.org/wargames/bandit/bandit0.html)

## **level Goal**
The goal of this level is for you to log into the game using SSH. The host to which you need to connect is bandit.labs.overthewire.org, on port 2220. The username is bandit0 and the password is bandit0. Once logged in, go to the Level 1 page to find out how to beat Level 1.

## **Walkthrough**
<details>
- <summary> Perform a SSH (Secure Shell) Connection</summary>
    - Figure out how to connect to ssh host with ssh user bandit0
</detials>
<details>
- <summary> Bandit uses port 2220 instead of port 22 </summary>
    - Figure out how to add a custom port to the ssh connection command
</detials>
<details>
- <summary> Use the given password and connect to the server</summary>
    - password: bandit0
</detials>

<detials>

<summary>## **Level 0 Command**</summary>
ssh bandit0@bandit.labs.overthewire.org -p 2220 
password bandit0
</details>