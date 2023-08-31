# 3108 2023 CTF Writeups
* notes
  - This is not an official writeups for 3108CTF. I just made it for fun.
  - This is just simple solution how I solve some of the ctf challenge.
  - Sorry for my bad writing for explaining the challenge.
 
## Table of contents
- [WEB - Lemah (Mudah)](#web---lemah-mudah)
- [WEB - Wantujus (Mudah)](#web---wantujus-mudah)
- [WEB - Wantusom (Sederhana)](#web---wantusom-sederhana)
- [WEB - Pantun Pantul (Sederhana)](#web---pantun-pantul-sederhana)
- [WEB - Warganegara (Sederhana)](#web---warganegara-sederhana)
- [WEB - Bendera (Mudah)](#web---bendera-mudah)
- [REVERSE ENGINEERING - Sarawak (Mudah)](#reverse-engineering---sarawak-mudah)
- [STEGA - Tugu Negara (Sederhana)](#stega---tugu-negara-sederhana)
- [STEGA - Jalur Gemilang (Mudah)](#stega---jalur-gemilang-mudah)
- [STEGA - Bangsal 1 (Sederhana)](#stega---bangsal-1-sederhana)
- [STEGA - Hari Keramat (Mudah) - Reupload](#stega---hari-keramat-mudah---reupload)
- [STEGA - Uncover (Sederhana)](#stega---uncover-sederhana)
- [CRYPTOGRAPHY - Nasihat (Mudah)](#cryptography---nasihat-mudah)
- [CRYPTOGRAPHY - Selamat Malam (Sederhana)](#cryptography---selamat-malam-sederhana)
- [CRYPTOGRAPHY - Keretapi Tanah Melayu 🚂 (Mudah)](#cryptography---keretapi-tanah-melayu--mudah)
- [CRYPTOGRAPHY - Jerebu (Sederhana)](#cryptography---jerebu-sederhana)
- [CRYPTOGRAPHY - 1957bit (Sederhana)](#cryptography---1957bit-sederhana)
- [NETWORK - Johan (Mudah)](#network---johan-mudah)
- [NETWORK - Lagi-Lagi Johan (Mudah)](#network---lagi-lagi-johan-mudah)
- [NETWORK - Jalan Jalan Di Kuala Lumpur (Mudah)](#network---jalan-jalan-di-kuala-lumpur-mudah)
- [NETWORK - Perpaduan (Mudah)](#network---perpaduan-mudah)
- [MISC - Mencari Rahsia Si Dia (Mudah)](#misc---mencari-rahsia-si-dia-mudah)
- [MISC - Pesan Tentang Bicara (Sederhana)](#misc---pesan-tentang-bicara-sederhana)
- [MISC - 3108 CTF Town (Sederhana)](#misc---3108-ctf-town-sederhana)
- [MISC - Nasi Lemak 1 Juta (Mudah)](#misc---nasi-lemak-1-juta-mudah)
- [FORENSICS - Negeri-Negeri Di Malaysia (Mudah)](#forensics---negeri-negeri-di-malaysia-mudah)
- [FORENSICS - Hatta (Sederhana)](#forensics---hatta-sederhana)
- [OSINT - Pertemuan Kapista : Babak I (Mudah)](#osint---pertemuan-kapista--babak-i-mudah)
- [OSINT - Hero Melayu (Mudah)](#osint---hero-melayu-mudah)
- [OSINT - Kisah Lama (Mudah)](#osint---kisah-lama-mudah)
- [OSINT - Pertemuan Kapista : Babak II (Mudah)](#osint---pertemuan-kapista--babak-ii-mudah)
- [OSINT - Mesej Dalam Botol (Sederhana)](#osint---mesej-dalam-botol-sederhana)
- [OSINT - Pertemuan Kapista : Finale (Mudah)](#osint---pertemuan-kapista--finale-mudah)
- [OSINT - Saya Di Mana (Mudah)](#osint---saya-di-mana-mudah)

## WEB - Lemah (Mudah)

- view source code, goto auth.js, find the code, decode using [cyberchef](https://cyberchef.org/#recipe=Magic(3,false,false,'')&input=NTEsNDksNDgsNTYsMTIzLDExMiw1MiwxMTUsMTE1LDExOSw0OCwxMTQsMTAwLDk1LDEwOCw1MSwxMDksNTIsMTA0LDMzLDEyNQ)

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/bd541c73-c622-4e1a-8e6a-a0bd47895d5a)

## WEB - Wantujus (Mudah)

- keep spamming until you win 10, check cookie, decode using [cyberchef](https://cyberchef.org/#recipe=Magic(3,false,false,'')&input=TXpFd09IdGlhWE5yZFhSZmJXRnlhV1Y5)

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/28a07fc9-6132-4395-8e9a-d2c302ac9f8c)

## WEB - Wantusom (Sederhana)

- keep spamming until you win 9 rounds (this is unbeatable to win 10 rounds), run the function that return a random choice, this means that the computer will no longer be able to always win on the 9th win
![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/c74a4cc8-c4d9-41eb-8b56-c058d114a71a)

- check cookie, decode using [cyberchef](https://cyberchef.org/#recipe=Magic(3,false,false,'')&input=TXpFd09IdGlhWE5yZFhSZmRHbG5aWEo5)

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/e0ad2188-fe2b-411c-8c58-b40c30961645)

## WEB - Pantun Pantul (Sederhana)

- just enter any value and submit, run the function `bendera()`

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/7d3cf884-7f96-4860-9f4b-3d9c6b11b920)

## WEB - Warganegara (Sederhana)

- using curl in terminal `curl -H "x-country-code: MY" https://warganegara.bahterasiber.my`

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/c777015a-5a0b-4c10-b7ad-e57a3e061e9f)

## WEB - Bendera (Mudah)

- edit request `bendera[]=bendera`

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/b0065e58-b04f-4777-892b-27efda6da39a)

## REVERSE ENGINEERING - Sarawak (Mudah)

- view strings

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/bb0b44c9-e228-457d-bd83-50a131063643)

## STEGA - Tugu Negara (Sederhana)

- view strings

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/55555799-bc78-4c73-be6f-17178a2dab87)

## STEGA - Jalur Gemilang (Mudah)

- using HxD, you need to repair some header

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/d5f32b10-3789-4fc7-ae7a-d19f20ea4f3d)

- based on other example, the header must be like this

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/c1bbdcbf-8c8e-41ed-8996-67eb35f174ed)

- open the edited header

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/fa59b998-92d2-4d76-98b4-84390815de8c)

## STEGA - Bangsal 1 (Sederhana)

- decode using [Steganographic Decoder](https://futureboy.us/stegano/decinput.html) without password you will get the second picture

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/50d4dc1e-e1a4-4d70-b277-c2bbfd985b1b)

- decode again using [Steganographic Decoder](https://futureboy.us/stegano/decinput.html) but this time using password `kemerdekaan`

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/eb60ed7e-f302-41da-8c97-cf297ea9bc80)

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

- open file using wireshark then export the file `File -> Export Objects -> HTTP`

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/d2591066-2305-4ac3-a07c-276b701826aa)

- open file `newuser.php` then decode all the binary using [ascii code](https://www.dcode.fr/ascii-code) you will get a link

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/c5abdea9-1ce8-42bc-8812-82679424c14a)

- open the link, find the flag

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/675401cf-dd42-4862-b4b3-69a895ae507f)

## NETWORK - Lagi-Lagi Johan (Mudah)

- open file using wireshark then export the file `File -> Export Objects -> HTTP`

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/5bc6ceaf-d10c-44a1-a146-2de447689a30)

- open file `newuser(1).php`, I think this is the flag, sorry dont remember

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/6342e63c-3b02-4595-96cb-3bbcf15a48d4)

## NETWORK - Jalan Jalan Di Kuala Lumpur (Mudah)

- open file using wireshark then export the file `File -> Export Objects -> HTTP`

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/5f1daa2f-00d6-4cf0-abef-9a740b9b910b)

- open file `.----%20-----.pdf` you will get part of flag

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/ae9f4a3b-8e91-474d-ade3-1744ad12fbb1)

- open file `flag.txt` you will get another part of flag

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/3053799f-615f-460a-a1ca-0ff5881d5683)

- open file `galeri.png` you will get another part of flag

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/9a2bd010-d2c5-4d1c-9b62-03787d42b726)

## NETWORK - Perpaduan (Mudah)

- combine the the given text at the top of website to become a link `app.mediafire.com/stc0yhefz10a6`

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/30e876f5-f6d5-495e-89f5-53c0f3b5f900)

- download file `3108.txt`

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/9eaba9b5-c554-44c2-89ff-5b5db8b467fe)

- open and find the flag, there are many fake flag you need to find the right flag at line `14350600`

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/9f459ed8-6cc4-49e9-aed6-7ea8258814de)

## MISC - Mencari Rahsia Si Dia (Mudah)

- decode using [spam mimic](https://spammimic.com/decode.shtml)

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/0084a147-dfee-4e90-b2da-d9c866b664b2)

## MISC - Pesan Tentang Bicara (Sederhana)

- extract the morse code and decode using [morse code translator](https://www.dcode.fr/morse-code)

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/e5c79b93-7222-443f-90a4-9c3b644243a3)

- decode using [vigenere cipher](https://www.dcode.fr/vigenere-cipher) with key `KEY`

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/cd4eac40-3cbc-4da2-b2a8-4c1e2b1cea74)

## MISC - 3108 CTF Town (Sederhana)

- open the game using `Visual Boy Advance - Game Boy Advance (GBA) Emulator` or another familiar software, and speedrun game to this part

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/47a513f9-c1e2-4012-b081-eaad4c090e50)

## MISC - Nasi Lemak 1 Juta (Mudah)

- from the hint you need to find the `bahan rahsia`. so i maximize the software and found the secret

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/bcc3a5c7-7f5a-44ef-9d2f-add44d1bb6b7)

- using cheat engine to modify the value

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/f7150f0d-8c03-4701-bcb4-670ed7d3ec49)

- click `bahan rahsia` and popout

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/ca1f7c8c-b5fd-48b0-a11f-c65c0f11b0d1)

## FORENSICS - Negeri-Negeri Di Malaysia (Mudah)

- view strings

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/b61c4d1a-3c0f-44c3-994f-02ab3ec23730)

- decode using [cyberchef](https://cyberchef.org/#recipe=Magic(3,false,false,'')&input=TXpFd09Ic3hSRE5PVkRGVU1WOU5ORXcwV1ZNeE5IMD0)

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/2b9efb6a-6897-408f-95be-3fd6591c80f9)

## FORENSICS - Hatta (Sederhana)

- view strings

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/00d53108-81ff-4108-9a3a-c4174d8a0117)

- decode using [special tool](https://cyberchef.org/#recipe=Find_/_Replace(%7B'option':'Simple%20string','string':'.'%7D,'0',true,false,true,false)Find_/_Replace(%7B'option':'Regex','string':'/'%7D,'1',true,false,true,false)From_Binary('None',8)&input=Li4vLy4uLy8uLi8vLi4uLy4uLy8uLi4uLi4vLy8uLi4uLy8vLy4vLy4vLy4vLi8vLi4vLy4uLy8uLy8uLi4vLy4vLy4vLi4vLi8vLi8vLi4uLy4vLy8vLy4vLy4uLi8vLi8vLi8uLi8uLy8uLy8uLi4vLy4vLi4vLi8uLy8vLy8uLy8vLi4uLi4uLy8uLy4uLi8vLi4vLi4uLy8uLy4uLy4vLy8vLy4v) , actually you need to replace `.` into `0` and `/` into `1`

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/d47c7c73-d8cd-45b1-a7e6-9dd4a6426858)

## OSINT - Pertemuan Kapista : Babak I (Mudah)

- open the given link [youtube](https://www.youtube.com/watch?v=ydDS01hfqQk)

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/d634c926-2791-4a76-923c-5997f7cd6809)

- open X / twiter [madah4arjuna](https://twitter.com/madah4arjuna)

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/ce87c079-1de8-4854-8693-52c7b33c9ef4)

## OSINT - Hero Melayu (Mudah)

- open tiktok [@pempengaruhsiber](https://www.tiktok.com/@pempengaruhsiber)

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/80c1ad38-a4f6-4399-9694-171c22db7d38)

- open this video and boom

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/5e832fc6-5f08-4a03-9958-13664b57fee5)

## OSINT - Kisah Lama (Mudah)

- using [wayback machine](https://web.archive.org/) to find `kisah silam lama yang tidak dilupai`

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/d583ac00-a5e0-4574-96e8-be9d17fc2f16)

## OSINT - Pertemuan Kapista : Babak II (Mudah)

- this chal is related to Babak I
- you need to decode the strings from the x / twitter 
- before decode you need to combine the strings

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/8ecb9130-832a-4bcd-89fd-86d9b786878c)

- open telegram and find `lanang kusrani`

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/d84062fd-ac33-448a-a0a4-3aa7d6ffcefe)

## OSINT - Mesej Dalam Botol (Sederhana)

- based on clue, you need to find the name and year, because you need it to unlock file zip/rar file
- using google images you found the name `Bahtera Pertiwi`

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/86f769b0-d604-427f-a3d2-1975a39d22d4)

- using yandex images, just try my luck and get the year `2014`

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/e5d5a2aa-596b-4792-b84c-ecafc1eda385)

- so the password is `BAHTERAPERTIWI_2014` extract the file

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/f2214159-d685-4ea8-8317-9fc2e780bf88)

- open the file and decode part of hidden strings == b\`_gLsb(\`Oz\`#c}cN

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/66015b45-1063-42c3-bc44-1639bf51d6ed)

- decode using [ROT 47](https://www.dcode.fr/rot-47-cipher)

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/ae0073b2-d3e9-4d20-a1ec-771daf1eccb1)

## OSINT - Pertemuan Kapista : Finale (Mudah)

- this chal is related to Babak II
- you need to to open instagram from the telegram

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/06be6039-3dbe-4d23-a9a5-a28df4aec393)

- click on this picture you will get hidden strings

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/ddd1652c-a565-4f1c-b33d-ccc6b06c6e99)

- extract the string and decode using [base 64](https://www.base64decode.org)

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/cc4d0d5e-581b-428e-91ae-64ace3567dfe)

- open the link and you need to find the password

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/56e6492f-c6d1-4421-a0f2-cd8d850369f6)

- go back to instagram to find the clue

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/0fa74282-a779-491a-b7fd-3f2d2a2bd3cf)

- so the password is `31082023`

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/dbd4bff5-0a08-4b5d-94da-26076f0d024a)

## OSINT - Saya Di Mana (Mudah)

- this chal is so stressful because you need to know and find accurately the place
- I know this place somewhere in Melaka because I search the hotel `The Explorer`
- so the true place is `Dataran Pahlawan Melaka` and find the newest review from that place

![image](https://github.com/0hanif0/31082023CTF-Writeups/assets/23289982/b08434e6-6819-4359-bdd4-72be26a4b34a)

# THANK YOU
