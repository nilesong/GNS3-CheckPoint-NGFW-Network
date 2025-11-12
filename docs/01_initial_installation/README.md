[← Back to Main](../../) • [Next: GUI Configuration →](../02_gui_configuration)

# 🧩 Step 1: Check Point Initial Installation

This section covers the initial setup of the **Check Point Gaia appliance** inside your GNS3 topology.

---

### 🖥️ Steps

1. Power on the **Check Point appliance** in GNS3.

   <img width="641" height="535" alt="Screenshot 2025-11-12 005625" src="https://github.com/user-attachments/assets/9c633403-56bd-4519-bee8-2ea4a3c667af" />

2. Follow the on-screen installation prompts:
   - Set admin password → `adminpassword1234`
     
     <img width="719" height="458" alt="Password" src="https://github.com/user-attachments/assets/c681b5d3-11e2-4460-a07f-cbef6e70b155" />

   - Set IP Address → `192.168.1.99 / 255.255.255.0`
     
     <img width="721" height="457" alt="IP Address" src="https://github.com/user-attachments/assets/fb30b84c-3b84-4b56-af34-e79c1b0fe463" />

   - Reboot
     
3. From **Management-PC1**, open a browser and navigate to: `https://192.168.1.99`
   
   <img width="638" height="448" alt="Browser" src="https://github.com/user-attachments/assets/7e89329c-02b6-40f9-a5ba-f7060cac4daf" />

4. Complete the **First Time Setup Wizard**:
   - Assign `eth1` as **Internet**
     
     <img width="638" height="449" alt="eth1" src="https://github.com/user-attachments/assets/db4fb479-d82b-4d07-9769-461bba15a4ea" />

   - Choose **Security Gateway and/or Security Management**
     
     <img width="639" height="452" alt="Security Gateway-Security Management" src="https://github.com/user-attachments/assets/30229d06-ed74-46bc-bd29-23db924aa7a1" />

---

### ✅ Result

After reboot and setup completion, you should be able to reach the **Gaia Web Portal** via `https://192.168.1.99` and log in with your admin credentials.

---

[← Back to Main](../../) • [Next: GUI Configuration →](../02_gui_configuration)
