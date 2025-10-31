 # SSH Project

This project teaches the basics of SSH (Secure Shell) in Linux — how to connect to servers securely, generate SSH keys, and configure your SSH client for passwordless login.

---

## Project Structure

ssh/
├── 0-use_a_private_key  
├── 1-create_ssh_key_pair  
├── 2-ssh_config  
├── school  
└── school.pub  

---

## Task 0: Use a Private Key

**File:** `0-use_a_private_key`  
**Goal:** Connect to your server using the SSH private key.

**Requirements**
- Use private key `~/.ssh/school`
- Connect as user `ubuntu`
- Use only single-character flags (`-i`, `-o`, etc.)
- Cannot use `-l`
- No need to handle passphrase keys

**Example Script**
```bash
#!/bin/bash
ssh -i ~/.ssh/school ubuntu@<server_ip>
