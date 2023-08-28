# 3108 2023 CTF Writeups
* notes
  - This is not an official writeups for 3108CTF. I just made it for fun.
  - This is just simple solution how I solve some of the ctf challenge.
  - Sorry for my bad writing for explaining the challenge.

## WEB - Lemah (Mudah)

- view source code, goto auth.js, find the code, decode using [cyberchef](https://cyberchef.org/#recipe=Magic(3,false,false,'')&input=NTEsNDksNDgsNTYsMTIzLDExMiw1MiwxMTUsMTE1LDExOSw0OCwxMTQsMTAwLDk1LDEwOCw1MSwxMDksNTIsMTA0LDMzLDEyNQ)

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/bd541c73-c622-4e1a-8e6a-a0bd47895d5a)

## WEB - Wantujus (Mudah)

- keep spamming until you win 10, check cookie, decode using [cyberchef](https://cyberchef.org/#recipe=Magic(3,false,false,'')&input=TXpFd09IdGlhWE5yZFhSZmJXRnlhV1Y5)

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/28a07fc9-6132-4395-8e9a-d2c302ac9f8c)

## WEB - Wantusom (Sederhana)

- keep spamming until you win 9 rounds (this is unbeatable to win 10 rounds), run the function that return a random choice, this means that the computer will no longer be able to always win on the 9th win, check cookie, decode using [cyberchef](https://cyberchef.org/#recipe=Magic(3,false,false,'')&input=TXpFd09IdGlhWE5yZFhSZmRHbG5aWEo5)

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/c74a4cc8-c4d9-41eb-8b56-c058d114a71a)

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/e0ad2188-fe2b-411c-8c58-b40c30961645)

## WEB - Pantun Pantul (Sederhana)

- just enter any value and submit, run the function `bendera()`

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/7d3cf884-7f96-4860-9f4b-3d9c6b11b920)

## REVERSE ENGINEERING - Sarawak (Mudah)

- view strings

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/bb0b44c9-e228-457d-bd83-50a131063643)

## STEGA - Tugu Negara (Sederhana)

- view strings

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/55555799-bc78-4c73-be6f-17178a2dab87)

## STEGA - Hari Keramat (Mudah) - Reupload

- use [StegOnline](https://stegonline.georgeom.net/upload), click LSB Half, to see the hidden text `angKaRahs1a`

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/a74e26b0-5e22-4bbb-ad3f-1fc8508edb84)

- use [Steg Decoder](https://futureboy.us/stegano/decinput.html) with password `angKaRahs1a` to see embedded file with the hidden text

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/bc0a34d0-13dd-4c0e-8386-c3c53cd8396a)

- decode using [ROT 47](https://www.dcode.fr/rot-47-cipher)

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/f72f8bee-8728-491d-bd28-fa237e24506b)

## STEGA - Uncover (Sederhana)

- decode using [Hexahue](https://www.dcode.fr/hexahue-cipher)

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/6ed4fcde-7e67-4786-b1b7-d3171a2f51b1)

## CRYPTOGRAPHY - Nasihat (Mudah)

- view strings `nasihat.py` to see the password `1ng4t-rukun-n3g4ra`

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/178304b4-9682-4953-be1e-22a510c5b8ab)

- run the python with flag.txt.enc

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/1fd9add9-cd9a-49f1-bb66-deee2d6513c0)

## CRYPTOGRAPHY - Selamat Malam (Sederhana)

- decode using [atbash cipher](https://www.dcode.fr/atbash-cipher)

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/1829ba5c-fbaf-47d7-a8fb-134656ba912e)

- they are weird Capital Letter in the text, just separate the weird letters

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/2fa030ff-0d00-4597-8df7-4fb7c37a69dd)

## CRYPTOGRAPHY - Keretapi Tanah Melayu 🚂 (Mudah)

- decode using [Rail fence cipher](https://www.boxentriq.com/code-breaking/rail-fence-cipher)

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/7b8d960a-2bc0-41b3-b9cb-345a65c556c6)

## CRYPTOGRAPHY - Jerebu (Sederhana)

- just decode some of obviously part only using [Music Sheet Cipher](https://www.dcode.fr/music-sheet-cipher)

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/c4eea7bf-b0b2-4f1f-920f-53990eb82cdd)

## CRYPTOGRAPHY - 1957bit (Sederhana)

- decode using [XOR Cipher](https://www.dcode.fr/xor-cipher) with key `1957`

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/91dfdf6e-a76d-4617-9b6a-b33307a27b4d)

## NETWORK - Johan (Mudah)

- open file using wireshark then export the file `File -> Export Objects -> HTTP`, 

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/d2591066-2305-4ac3-a07c-276b701826aa)
