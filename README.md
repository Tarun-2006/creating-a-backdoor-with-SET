# creating-a-backdoor-with-SET
creating a backdoor with SET - Ethical Hacking Techniques course

### Developed by :-

### Name : Tarun S
### no: 212223040226

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

<img width="938" height="834" alt="image" src="https://github.com/user-attachments/assets/d85e5739-643f-4cf7-89e9-41fc18be60d4" />


**2. Navigate:**
```bash
1) Social-Engineering Attacks  
2) Website Attack Vectors  
3) Credential Harvester Attack Method  
```

<img width="957" height="720" alt="image" src="https://github.com/user-attachments/assets/b62b1dbc-f8ee-4551-b653-d64a66a20d9c" />

<img width="851" height="777" alt="image" src="https://github.com/user-attachments/assets/a665e068-4178-476c-95c3-92f12eb20ddc" />


**3. Enter your IP address as the attacker server.**
**4. Choose:**
```bash
2) Site Cloner
```
<img width="663" height="343" alt="image" src="https://github.com/user-attachments/assets/e8784074-0ef6-4b44-8f85-ca2ea9f0bb1d" />

**5. Enter the URL of the legitimate site ```(e.g., https://accounts.google.com)```**

<img width="843" height="199" alt="image" src="https://github.com/user-attachments/assets/e7f7e8b6-c6cf-4260-9dd4-7314075884cf" />


**6. Send the generated link to the victim.**

<img width="1278" height="842" alt="image" src="https://github.com/user-attachments/assets/bf05c7a1-c679-4f73-a78f-4d89d27bc1ee" />


**7. Once the victim logs in → their credentials are stored in:**
```bash
/var/www/html/
```
<img width="945" height="427" alt="image" src="https://github.com/user-attachments/assets/0f49e7ad-9b92-4b0b-bd59-4d303b47634c" />





## RESULT:
The Social Engineering Toolkit (SET) is used to create backdoor is  examined successfully
