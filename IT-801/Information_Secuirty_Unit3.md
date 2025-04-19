# **Unit III: Public Key Encryption**

## **Public Key Cryptosystems ke Principles**

Public Key Cryptosystems cryptography ki ek important category hai, jisme do different keys ka use hota hai: ek public key aur ek private key. Public key ko kisi bhi person ko easily share kiya ja sakta hai, jabki private key sirf owner ke paas hoti hai. Iska basic idea yeh hai ki jo data aapko secure karna hai usko aap encrypt kar sakte hain public key se, aur sirf private key ka owner usse decrypt kar sakta hai.

### **Encryption Aur Decryption**

Public Key Cryptosystem ka main feature yeh hota hai ki encryption aur decryption alag-alag keys se hota hai. Jab aap kisi ko message bhejte ho, toh aap unki public key se us message ko encrypt karte ho. Jab recipient ko message milta hai, toh woh apni private key se message ko decrypt kar sakta hai. Yeh technique secure hoti hai kyunki even agar koi aapki public key dekh le, woh aapka encrypted message nahi padh sakta.

### **RSA Algorithm**

RSA (Rivest-Shamir-Adleman) ek popular public-key cryptosystem hai jo large prime numbers ka use karta hai encryption aur decryption ke liye. RSA kaafi commonly use hota hai in practice for secure communication, especially internet par.

RSA algorithm ka basic principle yeh hai ki aap two large prime numbers choose karte ho, unko multiply karte ho, aur phir ek public aur private key generate karte ho based on these primes. Yeh process mathematically complex hota hai aur iske through aap secure data transmission kar sakte ho.

#### **Key Generation**

1. **Choose Two Large Prime Numbers**: Pehle aapko do large prime numbers choose karne padte hain, jo generally 100 digits ya usse zyada lambi hoti hain.
2. **Compute Modulus**: Dono primes ka product calculate karte hain (n = p * q), jo modulus hota hai.
3. **Compute Euler’s Totient Function**: Iske baad Euler’s totient function ko calculate karte hain.
4. **Generate Public and Private Keys**: Public key mein modulus aur exponent hota hai, aur private key ke liye ek inverse exponent hota hai jo modulus ke under exist karta hai.

#### **Encryption Aur Decryption**

- **Encryption**: Sender message ko public key ke sath encrypt karta hai.
- **Decryption**: Receiver private key ka use karke message ko decrypt karta hai.

### **Diffie-Hellman Key Exchange**

Diffie-Hellman ek key exchange protocol hai jo allow karta hai do parties ko ek shared secret key securely exchange karne ke liye over an insecure channel. Iska basic concept yeh hai ki dono parties apne respective private keys generate karte hain aur publicly exchange karte hain apni values, aur phir ek common shared secret key derive karte hain using the exchanged information.

Isse ye faida hota hai ki dono parties apna secret key secure exchange kar sakte hain bina kisi attacker ke intervene kiye. Yeh protocol RSA se thoda different hai kyunki yeh key exchange par focus karta hai, na ki encryption aur decryption par.

### **Elliptic Curve Cryptography (ECC)**

Elliptic Curve Cryptography (ECC) ek modern cryptography technique hai jo elliptic curves ki mathematical properties ko use karti hai. ECC ko design kiya gaya tha taaki smaller key sizes ke sath bhi strong security achieve ki ja sake. Yeh RSA aur Diffie-Hellman se zyada efficient hai aur use hota hai secure communication mein, especially mobile devices aur IoT devices mein.

ECC mein, aap ek elliptic curve equation choose karte hain aur phir keys ko generate karte hain us curve par. Yeh system computationally efficient hai, matlab chhoti key sizes ke sath bhi aap strong security achieve kar sakte ho.

---

## **Message Authentication and Hash Functions**

### **Authentication Requirements**

Authentication ka purpose yeh ensure karna hota hai ki message sender ki identity valid ho aur message mein koi tampering na hui ho. Jab aap kisi message ko receive karte ho, toh aapko yeh verify karna padta hai ki woh message actually usi person ne bheja hai jiska aap expect kar rahe the.

Authentication generally do cheezon pe focus karta hai:
1. **Message Integrity**: Yeh ensure karna ki message ko transfer ke dauran modify nahi kiya gaya ho.
2. **Sender Authentication**: Yeh ensure karna ki message sender ko pehchana jaa sakta hai.

### **Authentication Functions**

Authentication functions woh algorithms hote hain jo message ko authenticate karte hain. Inka kaam hota hai message ko verify karna aur yeh ensure karna ki woh tampered nahi hua.

Commonly used authentication functions mein se ek hai **Message Authentication Code (MAC)**. MAC algorithm message ke sath ek secret key ko bhi use karta hai taaki ensure kiya ja sake ki message authorized source se aa raha ho.

### **Message Authentication Codes (MACs)**

MAC ek short piece of information hota hai jo ek message ke sath attach kiya jata hai. Yeh ensure karta hai ki message ko na toh modify kiya gaya ho, aur na hi sender ki identity forge ki gayi ho. 

MACs generate karte waqt sender aur receiver ek common secret key share karte hain. Jab message bheja jata hai, toh message aur secret key ko ek saath use karke MAC generate kiya jata hai. Receiver jab message receive karta hai, toh woh same process follow karke MAC ko validate karta hai.

### **Hash Functions**

Hash functions ka use kisi bhi input ko fixed-length output (jo hash kehlaata hai) mein convert karne ke liye hota hai. Hash functions commonly use hote hain passwords ko store karne ke liye, aur digital signatures create karne ke liye. Jab aap kisi large input ko hash karte ho, toh output size fixed hota hai, chaahe input kitna bhi bada ho.

Hash functions ka main feature yeh hota hai ki unmein pre-image resistance hoti hai, matlab agar aapke paas ek hash value hai, toh aap us hash ke corresponding input ko guess nahi kar sakte.

### **Security of Hash Functions and MACs**

Hash functions aur MACs ki security yeh ensure karti hai ki woh tampering se protected ho, aur unka output kisi third party ke liye guess karna mushkil ho. In algorithms ko design karte waqt, unhe is tarah se design kiya jata hai ki woh cryptographically secure ho aur kisi bhi type ke attack se bach sakein.

---

## **Hash and MAC Algorithms**

### **Secure Hash Algorithm (SHA)**

Secure Hash Algorithm (SHA) ek family hai cryptographic hash functions ki. Yeh algorithms widely use hote hain message integrity check karne ke liye. SHA-1 se lekar SHA-256 tak kai versions hain, jisme se SHA-256 ko commonly use kiya jata hai.

SHA algorithm message ko 256-bit length ka hash generate karta hai. SHA ka use kisi bhi type ke data ko secure karne ke liye kiya ja sakta hai, jaise ki digital signatures, password storage, etc.

### **HMAC**

HMAC (Hashed Message Authentication Code) ek special type ka MAC hai jo ek hash function aur secret key ka combination hota hai. HMAC ka use message authentication ke liye hota hai, aur yeh ensure karta hai ki message ki integrity aur authenticity maintain ho.

---

## **Digital Signatures and Authentication Protocols**

### **Digital Signature Standard (DSS)**

Digital Signature Standard (DSS) ek framework hai jo digital signatures create karne ke liye use hota hai. Digital signatures allow karte hain kisi document ya message ki authenticity ko verify karne ke liye.

DSS ka basic principle yeh hota hai ki sender apni private key ka use karke message ko sign karta hai, aur receiver public key ka use karke signature ko verify karta hai. Isse yeh ensure hota hai ki message genuine hai aur usme koi tampering nahi hui hai.

---

## **Potential Questions**

1. **What are the basic principles of Public Key Cryptosystems?**
2. **Explain the working of RSA algorithm.**
3. **What is the Diffie-Hellman Key Exchange protocol and how does it work?**
4. **What is Elliptic Curve Cryptography (ECC) and how is it different from RSA?**
5. **What are the authentication requirements in cryptography?**
6. **What is a Message Authentication Code (MAC) and how does it work?**
7. **Explain the working and use cases of hash functions in cryptography.**
8. **What is HMAC and how is it different from other MAC algorithms?**
9. **What is a digital signature and how does the Digital Signature Standard (DSS) work?**
10. **What are the security concerns related to the use of cryptographic hash functions?**
