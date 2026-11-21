# password-cracking-jtr
Cracked a password-protected PDF using John the Ripper in Kali Linux
# 🔓 Password Cracking with John The Ripper

Cracked my first password-protected PDF using John the Ripper in Kali Linux as part of Network Walks Tools Lab - Week 3 PM2.

## 🎯 What I Did

I was given a locked PDF file and I had to recover its password and capture the flag inside it.

## 🛠️ Tools Used

- Kali Linux
- John the Ripper
- pdf2john
- rockyou.txt wordlist

## 📝 Steps

### 1. Extract Hash from PDF
```bash
pdf2john "My Locked PDF1.pdf" > hash1.txt
2. Fix Dependency Error
I got a pyhanko missing error, so I installed it:bashpip install pyhanko --break-system-packages
3. Crack the Passwordbashjohn --wordlist=/usr/share/wordlists/rockyou.txt hash1.txt4. Show Cracked Passwordbashjohn --show hash1.txt Result
4Successfully cracked the PDF password and captured Flag 1!
Output:javascript1 password hash cracked, 0 left
