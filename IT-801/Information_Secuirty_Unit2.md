# 🔐 Unit II - Block Ciphers and Data Encryption Algorithm

---

## 📦 Block Cipher Principles (Block Cipher ke Principles)

Block Cipher ek encryption method hai jisme data ko fixed-size ke blocks mein divide karke encrypt kiya jata hai. Har block ko ek key ke sath encrypt kiya jata hai.

- **Block size** usually hota hai 64 bits ya 128 bits.
- Same plaintext block = same ciphertext (agar key wahi ho)
- Deterministic nature se kuch issues ho sakte hain, isliye **modes of operation** use kiye jate hain (discussed later)

### 🔑 Key Principles:
- **Large key space** hone chahiye (brute-force attack se bachne ke liye)
- **Confusion and Diffusion** concepts use hote hain:
  - **Confusion**: Ciphertext ka relation key se complex bana dena.
  - **Diffusion**: Plaintext ka har bit multiple ciphertext bits ko affect kare.

---

## 🔐 The Data Encryption Standard (DES)

DES ek symmetric key block cipher hai jo 1977 mein standard bana. Ye:

- **Block size**: 64-bit
- **Key size**: 56-bit
- **Rounds**: 16 rounds ka Feistel structure use karta hai

### 🔄 DES Process:
1. Initial Permutation
2. 16 Rounds of processing with subkeys
3. Final Permutation

Encryption aur decryption almost same process use karte hain, bas subkeys reverse order mein hoti hain.

---

## 💪 The Strength of DES

### 🔐 Strength:
- Complex structure (16 rounds)
- Strong S-boxes for substitution
- Avalanche effect (small input change → big output change)

### ❌ Weakness:
- Key size chhoti hai (56-bit) → brute-force se crack ho sakti hai
- 1998 mein EFF ne DES crack karne wala machine banaya tha (less than 24 hrs)
- Aaj ke time mein DES insecure maana jata hai.

---

## 🧠 Differential and Linear Cryptanalysis

### 🔁 Differential Cryptanalysis:
- Analyze karta hai input difference aur uska impact ciphertext par kya hai
- Mainly **chosen-plaintext attack** mein use hota hai

### 📊 Linear Cryptanalysis:
- Plaintext, ciphertext aur key bits ke beech linear relation find karta hai
- **Known-plaintext attack** pe based hota hai

Ye dono techniques DES pe kaafi effective hain, isliye naye algorithms like **AES** banaye gaye.

---

## 🏗️ Block Cipher Design Principles

- **Number of Rounds**: Zyada rounds = zyada security
- **Key Size**: Large key = better brute-force resistance
- **Subkey Generation**: Strong key schedule
- **Round Functions**: S-boxes aur permutation for confusion/diffusion
- **Feistel Structure**: Same structure for encryption and decryption

---

## 🔄 Advanced Encryption Standard (AES)

AES DES ka successor hai. NIST ne 2001 mein AES ko standard banaya.

- **Block size**: 128-bit
- **Key sizes**: 128, 192, 256 bits
- **Structure**: Substitution-Permutation Network (SPN)

---

## 🧪 Evaluation Criteria of AES

NIST ne AES select karte waqt kuch criteria rakhe:

- **Security**: Resistance to all known attacks
- **Performance**: Fast on both hardware & software
- **Simplicity**: Easy to implement
- **Flexibility**: Suitable for multiple platforms

---

## 🧩 The AES Cipher

AES mein steps hote hain:

1. **AddRoundKey**
2. **SubBytes** (Substitution)
3. **ShiftRows** (Permutation)
4. **MixColumns** (Diffusion)

- Repeat for **10/12/14 rounds** based on key size
- **Last round mein MixColumns nahi hota.**

---

## 🔁 Multiple Encryption and Triple DES (3DES)

To improve DES:

- 3DES ka use hua jisme DES ko **3 baar apply** kiya jata hai:
  - **Encrypt → Decrypt → Encrypt**

- **Key size**:
  - 112 bits (2 keys) ya 168 bits (3 keys)

- **Problem**: Slow performance compared to AES

---

## 🔄 Block Cipher Modes of Operation

Block ciphers normally sirf ek block pe kaam karte hain. Multiple blocks handle karne ke liye modes of operation use hote hain:

| Mode | Description |
|------|-------------|
| **ECB (Electronic Code Book)** | Simple but insecure (same block = same ciphertext) |
| **CBC (Cipher Block Chaining)** | Previous ciphertext block ko XOR karte hain |
| **CFB (Cipher Feedback Mode)** | Self-synchronizing stream cipher banata hai |
| **OFB (Output Feedback Mode)** | Stream cipher jaisa, error propagation nahi hoti |
| **CTR (Counter Mode)** | High performance, parallelizable |

---

## 🔁 Stream Ciphers

- Stream Cipher mein: Plaintext bits ko ek ek karke encrypt kiya jata hai
- **Fast and low memory usage**
- **Example**: RC4

**Downside**: Poorly implemented stream cipher = easy to break

---

## 🤝 Confidentiality using Symmetric Encryption

- Symmetric encryption mein: Same key encryption aur decryption ke liye use hoti hai
- **Fast and efficient** hai
- Confidentiality maintain karta hai agar key secure rahe

**Examples**: AES, DES, 3DES

---

## ❓ Questions You May Be Asked:

- Explain block cipher principles with examples.
- What is DES and how does it work?
- Why is DES considered weak today?
- Differentiate between differential and linear cryptanalysis.
- What are key design principles of a secure block cipher?
- Explain the AES algorithm and its steps.
- What criteria were used to evaluate AES?
- What is Triple DES and how is it better than DES?
- Explain various modes of operation used with block ciphers.
- Compare stream cipher and block cipher.
- How does symmetric encryption ensure confidentiality?
