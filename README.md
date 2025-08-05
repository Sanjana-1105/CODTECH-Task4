# CODTECH-Task4
**Name:** SANJANA PUROHIT
**Company:** CODTECH IT SOLUTIONS
**ID:** CT08DL1470
**Domain:** Cyber Security & Ethical Hacking
**Duration:** 30th May to 30th July 2025
**Mentor:** Neela Kumar


# Task 2 – Advanced Encryption Tool

### 🔍 Objective
This is a Python-based file encryption and decryption tool using **AES-256 encryption**.  
The tool uses a password to derive a secure encryption key and allows safe encryption and decryption of any file.

---

### ⚙️ Technologies Used
- Python
- `cryptography`

---

### 🛠️ Features
- AES-256 encryption (symmetric)
- Password-based key generation using PBKDF2HMAC
- Secure random salt added to encrypted output
- Encrypts and decrypts any type of file
- CLI-based interface

---

### 📦 How to Run

## How to Encrypt a File

```bash
python encrypt_tool.py
```
- Enter the filename (e.g., `secret.txt`)
- Enter your password (input hidden)
- Output: `secret.txt.enc` (AES-256 encrypted file)

## How to Decrypt a File

```bash
python decrypt_tool.py
```
- Enter the encrypted filename (e.g., `secret.txt.enc`)
- Enter the **same password**
- Output: `secret.txt_decrypted.txt`

---  

## 📁 File Format
Encrypted file structure: `[SALT (16 bytes)] + [ENCRYPTED DATA]`  
The salt is stored with the encrypted file to allow secure key regeneration.
