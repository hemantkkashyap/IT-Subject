# **Unit V: System Security**

## **Intruders, Intrusion Detection, Password Management**

### **Intruders**

Intruders woh unauthorized users hote hain jo kisi system ya network mein ghusne ki koshish karte hain. Intruders ka main goal system ki security ko bypass karna, sensitive data ko access karna, ya system resources ko misuse karna hota hai. Intruders ko generally 2 categories mein divide kiya jata hai:

1. **External Intruders**: Yeh outsiders hote hain jo network ya system mein without permission ghusne ki koshish karte hain.
2. **Internal Intruders**: Yeh woh users hote hain jo apne internal access ka galat use karte hain aur unauthorized actions perform karte hain.

Intruders generally system vulnerabilities ka use karke unauthorized access gain karte hain, jisme weak passwords, unpatched software, ya exposed ports shamil hote hain.

### **Intrusion Detection**

Intrusion Detection ek process hai jisme suspicious activities ko detect karna hota hai jo system security ko compromise kar sakti hain. Intrusion Detection Systems (IDS) yeh monitor karte hain ki system ke andar koi unusual activity ya unauthorized access ho raha hai ya nahi.

IDS generally do types ke hote hain:

1. **Signature-based IDS**: Yeh known attacks ke signatures ko match karta hai. Agar koi attack match hota hai toh IDS alert generate karta hai.
2. **Anomaly-based IDS**: Yeh system ke normal behavior ko establish karta hai aur jab bhi abnormal behavior detect hota hai, yeh alert generate karta hai.

IDS ka main purpose real-time monitoring aur quick response provide karna hota hai taaki attackers ko system mein ghusne se roka ja sake.

### **Password Management**

Password management ek critical part hai system security ka. Weak passwords ka use hone se system easily compromise ho sakte hain. Password management ka purpose yeh ensure karna hota hai ki users strong passwords use karein aur unke passwords secure tareeke se store ho.

- **Password Complexity**: Password ko strong banane ke liye, usmein uppercase, lowercase letters, numbers, aur special characters hone chahiye.
- **Password Expiry**: Regular intervals par passwords ko change karna chahiye taaki security breaches ko prevent kiya ja sake.
- **Two-Factor Authentication (2FA)**: Password ke saath ek extra layer of security provide karne ke liye, 2FA ka use kiya jata hai. Ismein user ko apni identity verify karne ke liye ek second method (jaise OTP ya biometric) use karna padta hai.

---

## **Malicious Software: Types, Viruses and Related Threats, Virus Countermeasures**

### **Different Types of Malicious Software**

Malicious software, jo commonly "malware" ke naam se jaana jata hai, woh software hota hai jo kisi system ya network ko damage ya compromise karne ke liye design kiya jata hai. Malware ke types mein shamil hain:

1. **Viruses**: Yeh self-replicating programs hote hain jo apne aap ko file ya system ke through propagate karte hain.
2. **Worms**: Yeh viruses se similar hote hain, lekin worms ko kisi file ya program ki zaroorat nahi hoti. Yeh apne aap se network par spread ho jate hain.
3. **Trojans**: Yeh malicious software hota hai jo legitimate software jaise dikhai deta hai, lekin jab user isse run karta hai toh yeh system ko compromise kar leta hai.
4. **Spyware**: Yeh software hota hai jo users ke activities ko secretly monitor karta hai aur sensitive data ko collect karta hai.
5. **Ransomware**: Yeh malicious software hota hai jo system ya data ko encrypt kar leta hai aur usse unlock karne ke liye ransom demand karta hai.

### **Viruses and Related Threats**

Viruses system ko infect karne wale programs hote hain jo apne aap ko ek system se doosre system tak spread karte hain. Yeh system ke resources ko corrupt kar sakte hain, files ko delete kar sakte hain, ya user ki sensitive information chura sakte hain.

Viruses ka main threat yeh hai ki woh system performance ko slow karte hain, data integrity ko damage karte hain, aur financial losses bhi cause karte hain. Common virus threats mein file infector viruses, boot sector viruses, aur macro viruses shamil hain.

### **Virus Countermeasures**

Virus countermeasures mein mainly antivirus software ka use hota hai jo viruses ko detect aur remove karte hain. Kuch common virus countermeasures hain:

- **Antivirus Software**: Yeh software viruses ko detect karta hai aur unhe remove karne ka kaam karta hai.
- **Regular Updates**: Antivirus software ko regularly update karna padta hai taaki woh naye viruses aur malware ke against protect kar sake.
- **Backup Systems**: Regular backups maintain karna important hai, taaki virus attack ke baad system ko restore kiya ja sake.

### **DoS and DDoS Attacks**

**Denial of Service (DoS)** attack ek attempt hota hai system ko overload karne ka, taaki woh legitimate users ke liye available na ho sake. DoS attack mein system ke resources ko exploit karte hue system ko crash ya hang kar diya jata hai.

**Distributed Denial of Service (DDoS)** attack DoS attack ka extended version hota hai. Isme multiple compromised systems (botnets) ka use hota hai jo ek hi time par target system par attack karte hain. Yeh attack zyada powerful aur difficult to defend hota hai.

Countermeasures against DoS/DDoS attacks include:

- **Traffic Filtering**: Suspicious traffic ko filter karna taaki woh attack execute na ho sake.
- **Rate Limiting**: Ek certain rate ke upar incoming traffic ko limit karna.
- **Intrusion Detection Systems**: IDS ka use DoS/DDoS attack ko detect karne ke liye kiya jata hai.

---

## **Security Controls for Information Security**

Information security ko protect karne ke liye kai tarah ke security controls use kiye jate hain. Inme physical, administrative, aur technical controls shamil hote hain.

### **Physical Controls**
- **Access Control**: Sensitive areas ko unauthorized access se protect karna.
- **Surveillance Systems**: CCTV cameras aur monitoring systems ka use hota hai taaki physical threats ko detect kiya ja sake.

### **Administrative Controls**
- **Policies and Procedures**: Security policies banani chahiye jo user behavior aur system access ko define karti hain.
- **Training and Awareness**: Users ko security best practices ke bare mein educate karna zaroori hai.

### **Technical Controls**
- **Encryption**: Data ko encrypt karna taaki woh unauthorized access ke liye unreadable ho jaye.
- **Access Control Lists (ACLs)**: ACLs ka use kiya jata hai taaki user access ko limit kiya ja sake.

---

## **Firewalls: Firewall Design Principles, Trusted Systems**

### **Firewall Design Principles**

Firewalls ek security system hain jo network traffic ko monitor aur control karte hain. Firewalls ka main purpose yeh hota hai ki woh unauthorized access ko prevent karein aur system ko internal aur external threats se protect karein.

Firewall design principles mein following important factors hote hain:

- **Least Privilege**: Firewalls ko minimum necessary permissions dena chahiye taaki system ko unnecessary access se protect kiya ja sake.
- **Layered Security**: Multiple layers of security use karna zaroori hota hai, jaise ki firewall, intrusion detection systems, aur encryption.
- **Traffic Filtering**: Firewalls traffic ko inspect karte hain aur suspicious packets ko drop karte hain.

### **Trusted Systems**

Trusted systems woh systems hote hain jo untrusted environments mein securely operate karne ke liye designed hote hain. In systems ko aise security features hote hain jo system ke integrity, confidentiality, aur availability ko ensure karte hain.

### **Common Criteria for Information Technology Security Evaluation**

Common Criteria (CC) ek standard hai jo IT security products ki evaluation ko define karta hai. Yeh evaluation process mein security assurance levels (EALs) define kiye jate hain, jo product ki security strength ko measure karte hain.

---

## **Potential Questions**

1. **What are the different types of malicious software and how can they affect system security?**
2. **Explain the working of Intrusion Detection Systems (IDS).**
3. **How can DoS and DDoS attacks be mitigated?**
4. **What are the best practices for password management in an organization?**
5. **Discuss the various countermeasures for virus attacks.**
6. **Explain the firewall design principles and their importance in system security.**
7. **What are trusted systems and how do they ensure secure operation?**
8. **What are the Common Criteria for information technology security evaluation?**
9. **How can system administrators detect and defend against intrusion attempts?**
10. **What are the different security controls required to protect information security?**
