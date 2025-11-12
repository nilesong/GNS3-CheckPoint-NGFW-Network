# 🧩 Step 3: SmartConsole Configuration

[← Previous: GUI Configuration](../02_gui_configuration) • [Back to Main README](../../)

This section covers setting up network objects, NAT, and security policies in **Check Point SmartConsole**.

---

### 💾 Initial SmartConsole Setup

1. Download and install **SmartConsole** from the Gaia Web GUI.  
2. Open SmartConsole and connect to your management server (`192.168.1.99`).

---

### 🌐 Network & NAT Configuration

1. Run **“Get Interfaces with Topology”** on your gateway.  
2. Enable **NAT**.  
3. Define Networks:
   - `LAN` → `eth2` → `192.168.0.0/24`  
   - `Management` → `192.168.1.0/24`

---

### 🛡️ Security Policies

1. Create an initial Internet policy to allow outbound access.  
2. Click **Install Policy**.  
3. Enable the following **Security Blades**:
   - Application Control  
   - URL Filtering  
   - IPS  
   - Anti-Bot  
   - Anti-Virus  
   - Content Awareness  
   *(Note: Demo mode may limit full functionality)*  
4. Add blades to your main policy filter.  
5. Define **Blocking Policies**:
   - Social Media: YouTube, Instagram, X/Twitter, etc.  
   - File Types: `.exe` and archive formats  
6. Enable **Logging** on all blocking policies.  
7. Click **Install Policy** again to apply.

---

### 📸 Suggested Screenshots

| Description | File Name |
|--------------|------------|
| Interface discovery | `smartconsole_01.png` |
| NAT settings | `smartconsole_02.png` |
| Network objects | `smartconsole_03.png` |
| Blade activation | `smartconsole_04.png` |
| Initial policy install | `smartconsole_05.png` |
| Blocking rules setup | `smartconsole_06.png` |
| Logging verification | `smartconsole_07.png` |
| Final policy install | `smartconsole_08.png` |

---

### ✅ Result

Once policies are installed and blades activated, the gateway will begin enforcing firewall, antivirus, and content policies — ready for testing using the URLs in the main README.

---

[← Previous: GUI Configuration](../02_gui_configuration) • [Back to Main README](../../)
