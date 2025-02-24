# Password-Cracking-and-Security

## Overview
This script automates password cracking using **John the Ripper** and **Hashcat**. It supports:
- **Automatic hash detection** using `hashid`
- **Dictionary and brute-force attacks**
- **Logging cracked passwords**
- **Extracting hashes from encrypted files**
- **GPU acceleration for faster cracking**

## Prerequisites
Ensure your system has the necessary tools installed:
```bash
sudo apt update
sudo apt install john hashcat python3-pip
pip install hashid
```
If cracking hashes from system files or ZIP archives:
```bash
sudo apt install unshadow zip2john
```

## Usage
### 1️⃣ Run the script:
```bash
chmod +x password_cracker.sh
./password_cracker.sh
```

### 2️⃣ Provide hash input:
- Enter the path to the **hash file**.
- The script detects hash type automatically.
- Choose **John the Ripper** or **Hashcat**.
- If using Hashcat, provide **hash mode ID** (suggested via `hashid`).

### 3️⃣ Select attack mode:
- **Dictionary Attack** (wordlist-based)
- **Brute-force Attack** (incremental character search)
- **Hybrid Attack** (wordlist + brute-force)

### 4️⃣ View results:
- Cracked passwords are stored in `cracked_passwords.log`.

## Example
```bash
./password_cracker.sh
```
📌 **Output example:**
```
[*] Detecting hash type...
[*] Cracking with John the Ripper...
[*] Cracked Passwords:
admin: P@ssw0rd123
```

## Features
✅ **Automatic Hash Detection**  
✅ **Multiple Attack Modes**  
✅ **GPU Acceleration for Hashcat**  
✅ **Extract Hashes from System & ZIP Files**  
✅ **Logging & Report Generation**  



## Author
🔹 **Cyberdeejah**  Penetration Tester

---
🚀 **Contribute:** Fork & improve this script! PRs welcome!

