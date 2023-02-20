# Pico Practice GYM

Writeups for Pico Practice General Category [pico ctf general category](https://play.picoctf.org/practice?category=5&page=1)

## **Obedient Cat**
```console
wget https://mercury.picoctf.net/static/217686fc11d733b80be62dcfcfca6c75/flag 
cat flag
```

## **Python Wrangling**
``` 
wget https://mercury.picoctf.net/static/8e33ede04d02f3765b8c6a6e24d72733/ende.py
wget https://mercury.picoctf.net/static/8e33ede04d02f3765b8c6a6e24d72733/pw.txt
wget https://mercury.picoctf.net/static/8e33ede04d02f3765b8c6a6e24d72733/flag.txt.en
echo "File Password:"
cat pw.txt
python3 ende.py -d flag.txt.en
```
## **Wave a Flag**
``` 
wget https://mercury.picoctf.net/static/a14be2648c73e3cda5fc8490a2f476af/warm
chmod +x warm
./warm -h
```

## **Nice Netcat**
```
nc mercury.picoctf.net 43239 >> flag.txt
python3 -c "filename = 'flag.txt'  # replace with the name of your file
lines = []

with open(filename, 'r') as f:
    for line in f:
        lines.append(line.strip())

text = ''
for x in lines:
    text += chr(int(x))
print(text)
"
```
## **Static ain't always noise**
```
wget https://mercury.picoctf.net/static/bc72945175d643626d6ea9a689672dbd/static
wget https://mercury.picoctf.net/static/bc72945175d643626d6ea9a689672dbd/ltdis.sh
chmod +x ltdis.sh
./ltdis.sh static
cat static.ltdis.strings.txt | grep "pico"
```

## **Tab, Tab, Attack**
``` 
wget https://mercury.picoctf.net/static/659efd595171e4c40378be6a2e9b7298/Addadshashanammu.zip
unzip Addadshashanammu.zip
./Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku/fang-of-haynekhtnamet
```

## **Magikarp Ground Mission**
```
echo "password is: 6d448c9c"
ssh ctf-player@venus.picoctf.net -p 59579
cat 1of3.flag.txt /2of3.flag.txt ~/3of3.flag.txt >> flag.txt
tr -d '\n' < flag.txt 
```

## **Lets Warm Up**
```
python3 -c "print('picoCTF{%s}'%(chr(int('0x70',16))))"
```

## **Warmed Up**
```
python3 -c "print('picoCTF{%s}'%(str(int('0x3D',16))))"
```

## **2Warm**
```
python3 -c "print('picoCTF{' +'{0:b}'.format(int(42)) +'}')"
```

## **What's a net cat?**
```
nc jupiter.challenges.picoctf.org 25103
```

## **Strings it**
``` 
wget https://jupiter.challenges.picoctf.org/static/94d00153b0057d37da225ee79a846c62/strings
strings strings | grep "picoCTF"
```

## **Bases**
``` 
python3 -c "import base64
base64_message = 'bDNhcm5fdGgzX3IwcDM1 '
base64_bytes = base64_message.encode('ascii')
message_bytes = base64.b64decode(base64_bytes)
message = message_bytes.decode('ascii')
print('picoCTF{%s}'%(message))"
```

## **First Grep**
```
wget https://jupiter.challenges.picoctf.org/static/315d3325dc668ab7f1af9194f2de7e7a/file
cat file | grep "picoCTF"
```

## **Codebook**
```
wget https://artifacts.picoctf.net/c/102/code.py
wget https://artifacts.picoctf.net/c/102/codebook.txt
python3 code.py
```

## **convertme.py**
``` 
wget https://artifacts.picoctf.net/c/31/convertme.py
echo "change to if True"
nano convertme.py
python3 convertme.py
```

## **fixme1.py**
``` 
wget https://artifacts.picoctf.net/c/39/fixme1.py
echo "fix print identidatiion error"
nano fixme1.py
python3 fixme1.py
```

## **fixme2.py**
``` 
wget https://artifacts.picoctf.net/c/65/fixme2.py
echo "fix to if ==''"
nano fixme2.py 
python3 fixme2.py
```

## **Glitch Cat**
```
nc saturn.picoctf.net 51109
python3 -c "print('picoCTF{gl17ch_m3_n07_' + chr(0x62) + chr(0x64) + chr(0x61) + chr(0x36) + chr(0x38) + chr(0x66) + chr(0x37) + chr(0x35) + '}')"
```