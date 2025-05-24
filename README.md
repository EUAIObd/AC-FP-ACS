# CryptoSuite: Applied Cryptography Final Project

### CSAC 329 – Applied Cryptography  
**Date:** May 2025

---

## 🎥 Presentation Links

- Part 1: https://youtu.be/IpBACxT-nQo
- Part 2: https://youtu.be/b5ujsr2Bvb4

---

## 👥 Group Members

- Eugene Aquilino – AES, UI Design
- John Michael Casila – RSA, Hashing
- Mary France San Andres – Documentation, File Support

---

## 📖 Introduction

CryptoSuite is a web-based application that demonstrates and applies modern cryptographic algorithms. Its purpose is to provide an interactive, educational platform for encrypting, decrypting, and hashing text and files. Cryptography is essential for protecting data confidentiality, integrity, and authenticity in today’s digital world, and this project aims to make these concepts accessible and practical for students and professionals.

---

## 🎯 Project Objectives

1. **Educational Demonstration:**  
   To provide a hands-on tool for learning and understanding symmetric and asymmetric encryption, hashing, and digital signatures.

2. **Practical Application:**  
   To enable users to securely encrypt, decrypt, and hash text and files using industry-standard algorithms.

3. **Security Awareness:**  
   To highlight common vulnerabilities in cryptographic applications and demonstrate best practices for secure implementation.

---

## 🏗️ Application Architecture & UI

CryptoSuite is built with a modular architecture using Python and Flask for the backend, and HTML, CSS (W3.CSS), and JavaScript for the frontend. The UI is designed to be modern, minimalist, and responsive, ensuring usability on both desktop and mobile devices.  
Navigation is organized by cryptographic function: Symmetric, Asymmetric, Hashing, and Algorithm Info. Each section provides clear forms for input and displays results and error messages in a user-friendly way.

---

## 🔐 Cryptographic Algorithms Implemented

### 1. **AES (Advanced Encryption Standard)**
- **Type:** Symmetric
- **Background:** Standardized by NIST in 2001, AES replaced DES as the primary symmetric cipher for government and industry.
- **How it works:** Encrypts data in fixed-size blocks (128 bits) using keys of 128, 192, or 256 bits. Uses rounds of substitution, permutation, and mixing.
- **Library:** PyCryptodome (`Crypto.Cipher.AES`)
- **Integration:** Used for text and file encryption/decryption in the Symmetric section.

### 2. **DES (Data Encryption Standard)**
- **Type:** Symmetric
- **Background:** Adopted in the 1970s, DES was the first widely used symmetric cipher but is now considered insecure due to its short key length.
- **How it works:** Encrypts 64-bit blocks with a 56-bit key using 16 rounds of permutation and substitution.
- **Library:** PyCryptodome (`Crypto.Cipher.DES`)
- **Integration:** Provided for educational purposes in the Symmetric section.

### 3. **3DES (Triple DES)**
- **Type:** Symmetric
- **Background:** Developed as a more secure alternative to DES by applying DES three times with different keys.
- **How it works:** Encrypts data by applying DES encryption, decryption, and encryption again (EDE mode).
- **Library:** PyCryptodome (`Crypto.Cipher.DES3`)
- **Integration:** Available for text and file encryption/decryption.

### 4. **RSA (Rivest–Shamir–Adleman)**
- **Type:** Asymmetric
- **Background:** Introduced in 1977, RSA is one of the first public-key cryptosystems and is widely used for secure data transmission.
- **How it works:** Uses a pair of keys (public/private) based on the difficulty of factoring large numbers. Supports encryption, decryption, and digital signatures.
- **Library:** Cryptography (`cryptography.hazmat.primitives.asymmetric.rsa`)
- **Integration:** Used for encrypting, decrypting, signing, and verifying messages in the Asymmetric section.

### 5. **ECC (Elliptic Curve Cryptography)**
- **Type:** Asymmetric
- **Background:** ECC offers strong security with smaller keys, making it efficient for mobile and embedded devices.
- **How it works:** Uses mathematical properties of elliptic curves over finite fields for key generation, encryption, and digital signatures.
- **Library:** Cryptography (`cryptography.hazmat.primitives.asymmetric.ec`)
- **Integration:** Used for ECC encryption and digital signatures.

### 6. **SHA-256 & SHA-512 (Secure Hash Algorithms)**
- **Type:** Hash
- **Background:** Part of the SHA-2 family, standardized by NIST. Widely used for data integrity and digital signatures.
- **How it works:** Produces a fixed-length hash (256 or 512 bits) from input data.
- **Library:** PyCryptodome (`Crypto.Hash.SHA256`, `Crypto.Hash.SHA512`)
- **Integration:** Used for hashing text and files in the Hashing section.

### 7. **MD5 (Message Digest 5)**
- **Type:** Hash
- **Background:** Once widely used, now considered insecure due to collision vulnerabilities.
- **How it works:** Produces a 128-bit hash value.
- **Library:** PyCryptodome (`Crypto.Hash.MD5`)
- **Integration:** Included for legacy and educational purposes.

### 8. **BLAKE2**
- **Type:** Hash
- **Background:** Modern hash function designed as a faster, secure alternative to MD5 and SHA.
- **How it works:** Produces variable-length hashes efficiently.
- **Library:** PyCryptodome (`Crypto.Hash.BLAKE2b`)
- **Integration:** Available for hashing text and files.

---

## 🖼️ Sample Runs / Outputs

### **AES Encryption Example**
**Input:**  
Text: `Hello World!`  
Key: `mysecretkey12345`  
Algorithm: AES

**Output:**  
```
U2FsdGVkX1+Q2k8k3Q==
```

### **RSA Encryption Example**
**Input:**  
Text: `Confidential Message`  
Public Key: *(auto-generated or user-provided)*

**Output:**  
```
Encrypted ciphertext (base64-encoded)
```

### **SHA-256 Hash Example**
**Input:**  
Text: `password123`

**Output:**  
```
ef92b778bafe771e89245b89ecbc08a44a4e166c06659911881f383d4473e94f
```

### **Screenshots**
*(Add screenshots of your UI for each section, e.g., symmetric encryption form, hashing form, output panels, etc.)*

```markdown
![Symmetric Encryption UI](screenshots/symmetric_ui.png)
![Hashing Output Example](screenshots/hashing_output.png)
```

---

## 🛠️ Technology Stack

- **Backend:** Python, Flask
- **Cryptography Libraries:** PyCryptodome, Cryptography
- **Frontend:** HTML, CSS (W3.CSS, custom), JavaScript
- **Deployment:** PythonAnywhere

---

## ⚙️ Setup Instructions

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/AC-FP-ACS.git
   cd AC-FP-ACS
   ```

2. **Create a virtual environment and activate it:**
   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the app:**
   ```bash
   python run.py
   ```
   Then open [http://localhost:5000](http://localhost:5000) in your browser.

---

## 🌐 Live Web Application

[https://ACACS.pythonanywhere.com](https://ACACS.pythonanywhere.com)

---


## 🙏 Acknowledgments

- [PyCryptodome Documentation](https://www.pycryptodome.org/)
- [Cryptography Library](https://cryptography.io/)
- [W3.CSS](https://www.w3schools.com/w3css/)
- [PythonAnywhere](https://www.pythonanywhere.com/)

---
