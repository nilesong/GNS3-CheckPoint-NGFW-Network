[← Previous: Initial Installation](../01_initial_installation) • [Back to Main README](../../) • [Next → SmartConsole Setup](../03_smartconsole_setup)

# 🧩 Step 2: Check Point GUI Configuration

This section details the interface and routing configuration performed in the **Gaia Web GUI** after the initial setup.

---

### ⚙️ Interface Configuration

1. Log in to the Gaia Web GUI at `https://192.168.1.99`.  
2. Navigate to **Network Management → Network Interfaces**.  
3. Configure:
   - **eth1** → Obtain IPv4 automatically (DHCP)  
   - **eth2** → `192.168.0.1 / 255.255.255.0`  
4. Save and apply changes.

---

### 🧭 Default Route

1. Go to **Network Management → Routing → Static Routes**.  
2. Add default route:
   - **Destination:** `0.0.0.0/0`  
   - **Next Hop:** `192.168.122.1`  
3. Click **Apply** to save changes.

---

### 📸 Suggested Screenshots

| Description | File Name |
|--------------|------------|
| eth1 DHCP setup | `gui_config_01.png` |
| eth2 static setup | `gui_config_02.png` |
| Default route configuration | `gui_config_03.png` |

---

### ✅ Result

The firewall should now have both **internal (LAN)** and **external (Internet)** connectivity, ready for policy setup in SmartConsole.

---

[← Previous: Initial Installation](../01_initial_installation) • [Back to Main README](../../) • [Next → SmartConsole Setup](../03_smartconsole_setup)
