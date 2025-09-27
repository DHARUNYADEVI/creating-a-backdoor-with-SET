# creating-a-backdoor-with-SET
creating a backdoor with SET - Ethical Hacking Techniques course

# AIM:
To Create a backdoor with Social Engineering Toolkit (SET)

## DESIGN STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode


### Step 2:

Investigate on the various categories of tools as follows:

### Step 3:

Open terminal and try execute some kali linux commands

### Architecture Diagram

```
+----------------+        +------------------------+        +----------------------+
| Attacker's PC  | -----> | SET (Credential        | -----> | Fake Login Page      |
| (Kali Linux)   |        | Harvester via Apache)  |        | (Hosted by SET)      |
+----------------+        +------------------------+        +----------------------+
       |                                                             |
       |                                                             v
       |   1. Configure SET with phishing site (e.g., Gmail clone)   |
       |                                                             |
       |                                                             v
       |                                                 +----------------------+
       |                                                 | Victim's Browser     |
       | <------------------------------------------------| Clicks Phishing Link|
       |                                                 +----------------------+
       |                                                             |
       |                                                             v
       |     2. Victim Enters Credentials → Sent to SET/Attacker    |
       |                                                             |
       |                                                             v
       |                                                 +----------------------+
       |                                                 | Credentials Captured |
       |                                                 | in Apache log/SET DB |
       |                                                 +----------------------+

```

## EXECUTION STEPS AND ITS OUTPUT:
Social Engineering attacks are the various cons used by the hackers to trick people into providing sensitive data to the attackers.

**Steps to Use SET for Phishing (Credential Harvester Attack Method)**

**1. Open terminal:**
```bash
sudo setoolkit
```
<img width="851" height="931" alt="Screenshot 2025-09-27 091602" src="https://github.com/user-attachments/assets/d2cf3d21-28f7-4e6b-becf-d852cb46fc74" />

**2. Navigate:**
```bash
1) Social-Engineering Attacks  
2) Website Attack Vectors  
3) Credential Harvester Attack Method  
```
<img width="703" height="376" alt="image" src="https://github.com/user-attachments/assets/b2a4de33-b90e-4400-a865-4e9ba47a13d5" />

<img width="1316" height="997" alt="Screenshot 2025-09-27 085806" src="https://github.com/user-attachments/assets/31f751a4-1f75-432e-803b-f03cfae31b16" />

<img width="1684" height="1042" alt="Screenshot 2025-09-27 085839" src="https://github.com/user-attachments/assets/d9bfe427-a3c1-4a68-8d3a-f12ed8a39c53" />

**3. Enter your IP address as the attacker server.**

<img width="797" height="468" alt="image" src="https://github.com/user-attachments/assets/fefbad2a-e592-4a39-9574-dbb1ffc4ba9c" />

**4. Choose:**
```bash
2) Site Cloner
```
<img width="790" height="504" alt="image" src="https://github.com/user-attachments/assets/676a0dfa-4b4b-46eb-b9e5-76dfd3160dac" />

**5. Enter the URL of the legitimate site ```(e.g., https://www.instagram.com)```**

<img width="1920" height="1080" alt="Screenshot (109)" src="https://github.com/user-attachments/assets/f680ad86-d518-44eb-adfd-352269d2b70f" />

<img width="1920" height="1080" alt="Screenshot (107)" src="https://github.com/user-attachments/assets/1c24ad42-be30-4708-a25c-16dfca3cabe9" />


**6. Send the generated link to the victim.**

<img width="794" height="470" alt="image" src="https://github.com/user-attachments/assets/cd02f71b-5f35-4ab7-a99d-4bc2ebb32add" />

**7. Once the victim logs in → their credentials are stored in:**
```bash
/var/www/html/
```
<img width="830" height="483" alt="image" src="https://github.com/user-attachments/assets/c387a68d-e9e4-4e8f-8c93-c02acff1abee" />

<img width="801" height="514" alt="image" src="https://github.com/user-attachments/assets/f69fb0f3-b927-4e37-853d-0d0747ce1543" />


## RESULT:
The Social Engineering Toolkit (SET) is used to create backdoor is  examined successfully
