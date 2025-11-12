# 🛡️ Check Point NGFW (Gaia) GNS3 Network

This repository contains the **Check Point Next Generation Firewall (NGFW)** setup running on **GNS3** using the **Checkpoint Gaia appliance**.  
The purpose of this lab is to simulate a functional firewall environment with **security blades**, **policy management**, and **threat prevention features** — all in a contained virtual lab environment.

---

## ⚠️ Notes

1. This repository **only includes the `.gns3` topology file**.  
   Due to legal and licensing restrictions, **no Check Point backups or image files** will be provided.  
2. Exporting full GNS3 project is **not feasible** because of file size limitations that exceed GitHub’s upload limits.  
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

> **Before you begin:**  
> Open the **`CheckPoint-NGFW.gns3`** file in GNS3.  
> This is the base project file containing the full topology layout.  
> All configuration steps below assume you have this project opened and running.

### Topology & IP Addressing

<img width="683" height="683" alt="Topology" src="https://github.com/user-attachments/assets/4e6f7622-40c5-4b8d-9cc0-c079581bd768" />

Follow the IP addressing and connection layout as shown in the topology diagram.<br>
Set your DNS Server to the IP address of the NAT node (`192.168.122.1` in this setup).

---

### Check Point GAiA Setup Guides

The setup portion is divided into three separate pages for clarity:

1. [Step 1: Check Point Initial Installation](docs/01_initial_installation/README.md)  
2. [Step 2: Check Point GUI Configuration](docs/02_gui_configuration/README.md)  
3. [Step 3: SmartConsole Configuration](docs/03_smartconsole_setup/README.md)

---

## 🧪 Testing & Verification

### Antivirus
Visit the EICAR test file to check Antivirus functionality:  
[http://www.eicar.org/download/eicar_com.zip](http://www.eicar.org/download/eicar_com.zip)

---

### Anti-Bot
Test Anti-Bot blade using the Check Point test page:  
[http://sc1.checkpoint.com/za/images/threatwiki/pages/TestAntiBotBlade.html](http://sc1.checkpoint.com/za/images/threatwiki/pages/TestAntiBotBlade.html)

<img width="838" height="465" alt="Blocked Antibot 1" src="https://github.com/user-attachments/assets/b8b661a3-71b6-4430-b424-7b6f242645b7" />

*Antivirus/Anti-bot blocked page.*

---

### Application & URL Filtering
Test access to blocked applications/websites:

- YouTube: `https://youtube.com`  
- Instagram: `https://instagram.com`  
- X/Twitter: `https://x.com`

<img width="838" height="527" alt="Blocked Website" src="https://github.com/user-attachments/assets/5cf5fb90-67ae-4edc-9353-210ed01e5913" />

*Website blocked page.*

### Log Entries

<img width="1300" height="529" alt="Logging" src="https://github.com/user-attachments/assets/bbe7ebb4-06a3-46a1-991c-e61bd930774b" />

*Log entries confirming the block.*

---

## 👤 Author

**Neil Ong**  
GitHub: [@nilesong](https://github.com/nilesong)

---

## 📄 License

This project is intended solely for non-commercial testing and research purposes.
All Check Point trademarks, names, and software are the property of Check Point Software Technologies Ltd.
