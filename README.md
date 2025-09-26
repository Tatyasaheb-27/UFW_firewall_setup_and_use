# 🔐 Cyber Security 

# Setup and Use a Firewall on Ubuntu

## 📌 Objective
Configure and test basic firewall rules using **UFW (Uncomplicated Firewall)** on Ubuntu to allow or block traffic.

---

## 🛠 Steps Performed

### Step 1: Install & Enable UFW

sudo apt update
sudo apt install ufw -y
sudo ufw enable
```

### Step 2: Check Status & List Rules

sudo ufw status verbose
sudo ufw status numbered
```

### Step 3: Block Inbound Traffic (Telnet, Port 23)

sudo ufw deny 23/tcp
sudo ufw status numbered
```

### Step 4: Test the Rule

telnet localhost 23
```
_Result: Connection refused (rule is working)._

### Step 5: Allow SSH (Port 22)

sudo ufw allow 22/tcp
sudo ufw status numbered
```

### Step 6: Remove Test Rule

sudo ufw status numbered
sudo ufw delete <rule_number>
```

---

## ✅ Outcome
- Learned **basic firewall management** using UFW.  
- Configured and tested firewall rules.  
- Gained understanding of **traffic filtering and security practices**.
