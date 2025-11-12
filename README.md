# 🛡️ Check Point NGFW (Gaia) GNS3 Homelab

This repository contains the **Check Point Next Generation Firewall (NGFW)** setup running on **GNS3** using the **Checkpoint Gaia appliance**.  
The purpose of this lab is to simulate a functional enterprise-grade firewall environment with **security blades**, **policy management**, and **threat prevention features** — all in a contained virtual lab environment.

---

## ⚠️ Notes

1. This repository **only includes the `.gns3` topology file**.  
   Due to legal and licensing restrictions, **no Check Point backups or image files** will be provided.  
2. Exporting full GNS3 projects is **not feasible** because of file size limitations that exceed GitHub’s upload limits.  
3. Instead, this repository provides:
   - The **topology overview**
   - **Step-by-step setup instructions**
   - Optional **screenshots** (added progressively in each setup step directory)

---

## 🧰 Requirements

Ensure you have the following installed and configured before starting:

1. **[GNS3](https://www.gns3.com/software/download)**  
2. **[GNS3 VM](https://www.gns3.com/software/download-vm)** (running on **VMWare Workstation** or **VMWare Fusion**)  
3. **GNS3 appliances and images** — see [`requirements.txt`](./requirements.txt) for all required appliances and image versions  

---

## ⚙️ Setup

### Topology & IP Addressing

Follow the IP addressing and connection layout as shown in the topology diagram.
Set your DNS Server to the IP address of the NAT node (`192.168.122.1` in this setup).

---

### Check Point GAiA Setup Guides

The setup portion is divided into three separate pages for clarity:

1. [Step 1: Check Point Initial Installation](docs/01_initial_installation/README.md)  
2. [Step 2: Check Point GUI Configuration](docs/02_gui_configuration/README.md)  
3. [Step 3: SmartConsole Configuration](docs/03_smartconsole_setup/README.md)

---

## 🧪 Testing & Verification

Use the following URLs to test the NGFW’s protection and policy enforcement:  

| Category | Test URL | Expected Result |
|-----------|-----------|----------------|
| **Antivirus** | [EICAR Test File](http://www.eicar.org/download/eicar_com.zip) | File blocked / alert logged |
| **Anti-Bot** | [Test Anti-Bot Blade](http://sc1.checkpoint.com/za/images/threatwiki/pages/TestAntiBotBlade.html) | Anti-Bot alert triggered |
| **Application & URL Filtering** | [YouTube](https://youtube.com) <br> [Instagram](https://instagram.com) <br> [X/Twitter](https://x.com) | Access blocked per policy, logs recorded |

📸 *(Screenshots: test_antivirus.png, test_antibot.png, test_urlfilter.png)*

---

## 🗂️ Repository Structure

