# 🧩 Step 1: Check Point Initial Installation

[← Back to Main README](../README.md) • [Next → GUI Configuration](02_gui_configuration.md)

This section covers the initial setup of the **Check Point Gaia appliance** inside your GNS3 topology.

---

### 🖥️ Steps

1. Power on the **Check Point appliance** in GNS3.  
2. Follow the on-screen installation prompts:
   - Set admin password → `adminpassword1234`  
   - Set IP Address → `192.168.1.99 / 255.255.255.0`  
   - Reboot  
3. From **Management-PC1**, open a browser and navigate to:  
   `https://192.168.1.99`
4. Complete the **First Time Setup Wizard**:
   - Assign `eth1` as **Internet**
   - Choose **Security Gateway and/or Security Management** roles

---

### 📸 Suggested Screenshots

| Description | File Name |
|--------------|------------|
| Initial console setup | `initial_install_01.png` |
| Password configuration | `initial_install_02.png` |
| IP address assignment | `initial_install_03.png` |
| Web GUI first-time setup | `initial_install_04.png` |
| Role selection | `initial_install_05.png` |

---

### ✅ Result

After reboot and setup completion, you should be able to reach the **Gaia Web Portal** via `https://192.168.1.99` and log in with your admin credentials.

---

[← Back to Main README](../) • [Next → GUI Configuration](../02_gui_configuration/README.md)