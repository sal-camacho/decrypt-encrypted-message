# Activity Overview

Previously, I learned about cryptography and how encryption and decryption can be used to secure information online. I was introduced to the Caesar cipher, one of the earliest cryptographic algorithms used to protect privacy. As a security analyst, it’s important to understand the role of encryption in securing data and to be familiar with the right security controls to do so. In this activity, I was guided through basic cryptographic tasks using Linux commands to decrypt files and reveal hidden messages.

## Scenario

In this scenario, all of the files in my home directory were encrypted. I needed to use Linux commands to break the Caesar cipher and decrypt the files so I could read the hidden messages they contained.

Here’s how I completed the task:
- Explored the contents of the home directory and read a file
- Found a hidden file and decrypted the Caesar cipher it contained
- Decrypted the encrypted data file to recover my data and reveal the hidden message

---
## Linux Cryptography — Decrypt an Encrypted Message

This report was completed as part of the Google Cybersecurity Certificate. It documents how to decrypt encrypted files using Linux Bash commands and classical cryptographic techniques. These tasks are essential for encryption workflows, secure data recovery, and foundational cryptographic principles.
## My Contributions

### Read the contents of a file

- Used `ls /home/analyst` to list files in the home directory  
- Used `cat README.txt` to read instructions  

### Find and decrypt a hidden file

Navigated to the `caesar` subdirectory using `cd caesar`  
- Listed hidden files with `ls -a`  
- Read `.leftShift3` using `cat .leftShift3`  
- Decrypted Caesar cipher using:
  ```bash
  cat .leftShift3 | tr "d-za-cD-ZA-C" "a-zA-Z"

## Tools Used

- ls — to list files
- cat — to read file contents
- cd — to navigate directories
- tr — to translate Caesar cipher text
- openssl — to decrypt AES-256-CBC encrypted file

## Reflections

- Reading encrypted instructions simulated real-world forensic analysis.
- Solving the Caesar cipher reinforced classical cryptography fundamentals.
- Using OpenSSL demonstrated practical symmetric encryption/decryption.
