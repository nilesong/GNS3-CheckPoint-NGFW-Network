[← Previous: Initial Installation](../01_initial_installation) • [Back to Main README](../../) • [Next: SmartConsole Setup →](../03_smartconsole_setup)

# 🧩 Step 2: Check Point GUI Configuration

This section details the interface and routing configuration performed in the **Gaia Web GUI** after the initial setup.

---

### ⚙️ Interface Configuration

1. Log in to the Gaia Web GUI at `https://192.168.1.99`.  
2. Navigate to **Network Management → Network Interfaces**.
   
   <img width="1612" height="509" alt="Interfaces" src="https://github.com/user-attachments/assets/113d1833-e1b6-4195-b3cf-00927ecaf3ca" />

3. Configure:
   - **eth1** → Obtain IPv4 address automatically (DHCP)
     
     <img width="461" height="372" alt="eth1" src="https://github.com/user-attachments/assets/41424458-894c-4122-8189-777aaf7c80aa" />

   - **eth2** → `192.168.0.1 / 255.255.255.0`
     
     <img width="461" height="376" alt="eth2" src="https://github.com/user-attachments/assets/11c9da4c-c1d5-47fb-8472-0ea1c31c5b93" />

4. Save and apply changes.

---

### 🧭 Default Route

1. Go to **Network Management → IPv4 Static Routes**.
   
   <img width="1245" height="428" alt="Default Route 1" src="https://github.com/user-attachments/assets/23344591-7658-471e-b244-218e6d3f98c4" />

2. Add default route:
   - **Gateway:** `192.168.122.1`
     
     <img width="423" height="562" alt="Default Route 2" src="https://github.com/user-attachments/assets/6302304e-8275-4cd6-a3f7-f5702704795b" />

3. Click **Save** to apply changes.

---

### ✅ Result

The firewall should now have both **internal (LAN)** and **external (Internet)** interfaces setup, ready for policy setup in SmartConsole.

---

[← Previous: Initial Installation](../01_initial_installation) • [Back to Main README](../../) • [Next: SmartConsole Setup →](../03_smartconsole_setup)
