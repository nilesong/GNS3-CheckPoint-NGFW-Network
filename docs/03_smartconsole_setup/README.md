[← Previous: GUI Configuration](../02_gui_configuration) • [Back to Main README](../../)

# 🧩 Step 3: SmartConsole Configuration

This section covers setting up network objects, NAT, and security policies in **Check Point SmartConsole**.

---

### 💾 Initial SmartConsole Setup

1. Download and install **SmartConsole** from the Gaia Web GUI.  
2. Open SmartConsole and connect to your management server (`192.168.1.99`).
   
   <img width="674" height="313" alt="SmartConsole" src="https://github.com/user-attachments/assets/80cd0eee-0046-47d4-b637-16c71b3448a2" />

---

### 🌐 Network & NAT Configuration

1. Run **“Get Interfaces with Topology”** on your gateway.

<img width="765" height="703" alt="Interfaces" src="https://github.com/user-attachments/assets/544b85ad-ae2d-4039-8e26-91eb4361e058" />

2. Enable **NAT**.

<img width="763" height="702" alt="NAT" src="https://github.com/user-attachments/assets/34c9d505-93b5-49c6-afbc-5849783c202d" />

3. Define Network & Hosts:
   - `LAN (Network)` → `eth2` → `192.168.0.0/24`
     
     <img width="1916" height="1040" alt="LAN 1" src="https://github.com/user-attachments/assets/da066e0b-86e9-4e11-9f76-4df631a33c98" />
     
     <img width="375" height="454" alt="LAN 2" src="https://github.com/user-attachments/assets/080c6c6c-dd99-4eb4-a8b2-21d4ef768f20" />
     
     <img width="375" height="454" alt="LAN 2" src="https://github.com/user-attachments/assets/3807bac6-c373-439a-b279-23cab0ed875e" />
     
   - `Management (Host)` → `192.168.1.0/24`
     
     <img width="1914" height="1034" alt="Management1" src="https://github.com/user-attachments/assets/7e14ea1e-46b1-4084-9b23-a39af3cb5489" />
     
     <img width="547" height="311" alt="Management2" src="https://github.com/user-attachments/assets/91a18c22-3c71-468b-932e-82ddc56cd72c" />
     
     <img width="548" height="416" alt="Management3" src="https://github.com/user-attachments/assets/80c7fb27-0288-4ca0-a10e-59bb9ba61e72" />

---

### 🛡️ Security Policies

1. Enable the following **Security Blades**:
   - Application Control  
   - URL Filtering  
   - IPS  
   - Anti-Bot  
   - Anti-Virus  
   - Content Awareness  
   *(Note: Demo mode may limit full functionality)*<br>
   <br>
   <img width="763" height="703" alt="Enable Blades" src="https://github.com/user-attachments/assets/0de6e537-1d7a-4858-b6a4-76029dbed337" />

2. Add blades to your main policy filter.
   
   <img width="1661" height="970" alt="Add Blades 1" src="https://github.com/user-attachments/assets/3b93d372-dce5-4414-8c00-559e34012091" />
   
   <img width="966" height="597" alt="Add Blades 2" src="https://github.com/user-attachments/assets/274da34f-86ad-46eb-b284-a0345cf3d8e5" />
   
   <img width="892" height="460" alt="Add Blades 3" src="https://github.com/user-attachments/assets/c9db899b-de8f-4e3d-9877-70f21b48680c" />
   
   <img width="970" height="600" alt="Add Blades 4" src="https://github.com/user-attachments/assets/53f1373d-d9d4-4f64-b6ce-03ed5763dfc6" />

3. Create an Internet policy to allow outbound access.
   
   <img width="1372" height="627" alt="Internet Policy" src="https://github.com/user-attachments/assets/c3cd0381-704c-48a1-a044-84d6f708648f" />

4. Define **Blocking Policies**:
   - Social Media: YouTube, Instagram, X/Twitter, etc.
   - 
     <img width="1372" height="627" alt="Social Media Policy" src="https://github.com/user-attachments/assets/0fa71915-1dc5-409b-87cb-78e782d0a2d9" />

   - File Types: `.exe` and archive formats
   - 
     <img width="1372" height="627" alt="File Type Policy" src="https://github.com/user-attachments/assets/2a06f8c7-b2a8-44f8-811f-9f1b2fc7b0cb" />

5. Enable **Logging** on all blocking policies.
   
   <img width="1372" height="627" alt="Logging" src="https://github.com/user-attachments/assets/d26342e4-ab65-4adc-854d-7940dab6f982" />

6. Click **Install Policy** to apply.

---

### ✅ Result

Once policies are installed and the security blades are activated, the gateway will begin enforcing firewall, antivirus, and content policies, while providing full internet and outbound connectivity. You can then proceed to verify functionality using the designated test URLs for each security blade.

---

[← Previous: GUI Configuration](../02_gui_configuration) • [Back to Main README](../../)
