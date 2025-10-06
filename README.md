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

<img width="745" height="458" alt="image" src="https://github.com/user-attachments/assets/6226ec93-4fbd-430f-9fd3-91dc8c6b62ff" />

<img width="891" height="585" alt="image" src="https://github.com/user-attachments/assets/8108fb81-9ae9-41a8-91be-533b87557903" />



**3. Enter your IP address as the attacker server.**
**4. Choose:**
```bash
2) Site Cloner
```
<img width="927" height="419" alt="image" src="https://github.com/user-attachments/assets/b28ed39d-2ebc-4e8f-ba7e-93875e8b5168" />


**5. Enter the URL of the legitimate site ```(e.g., https://accounts.google.com)```**

<img width="950" height="362" alt="image" src="https://github.com/user-attachments/assets/a0cc2fde-7ea0-4867-9854-d4ced959e73b" />



**6. Send the generated link to the victim.**

<img width="937" height="680" alt="image" src="https://github.com/user-attachments/assets/dddb777c-23ee-4744-8570-2425aa11baee" />




**7. Once the victim logs in → their credentials are stored in:**
```bash
/var/www/html/
```
<img width="847" height="227" alt="image" src="https://github.com/user-attachments/assets/11dd0556-7854-4f00-8bcc-d3c31edd0af1" />






## RESULT:
The Social Engineering Toolkit (SET) is used to create backdoor is  examined successfully
