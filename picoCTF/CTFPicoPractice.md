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

