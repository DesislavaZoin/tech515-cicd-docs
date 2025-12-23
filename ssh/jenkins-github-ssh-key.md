# Jenkins GitHub SSH Key Setup
- [Jenkins GitHub SSH Key Setup](#jenkins-github-ssh-key-setup)
  - [Purpose](#purpose)
  - [SSH Key Generation](#ssh-key-generation)
  - [Add Key to GitHub Repository](#add-key-to-github-repository)

## Purpose
To allow Jenkins to read from and push changes to the CICD repository over SSH.

---

## SSH Key Generation 
```bash
ssh-keygen -t rsa -b 4096 -C "desizzzzo@gmail.com"
```
- Generates a private key (`desi-jenkins-2-github-key`) and a public key (`.pub`)

## Add Key to GitHub Repository
1. Go to **GitHub → Settings → SSH and GPG keys** in the CICD repository.
2. Click **New SSH key**
3. Set:
    - **Title:** `desi-jenkins-2-github-key`
    - **Key:** contents of `desi-jenkins-2-github-key.pub`
4. Tick **Allow write access**
5. Click **Add key**
6. Confirm access or enter verification code from your email.