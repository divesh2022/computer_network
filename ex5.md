# 🖧 Implementation of Directory/File and Printer Sharing in Windows OS

## 🎯 Aim
To enable seamless sharing of files, folders, and printers across a local network using Windows OS, facilitating collaborative work and resource optimization.

---

## 📚 Theory
- File and Printer Sharing allows users to access resources on other computers within the same network.
- It uses protocols like **SMB (Server Message Block)** and **TCP/IP** for communication.
- This setup enhances collaboration, reduces redundancy, and centralizes resource management.

---

## 🧰 Requirements
- Two or more computers connected to the same **Local Area Network (LAN)**.
- **Windows OS** installed on all systems.
- A folder or printer to be shared.
- **Administrative privileges** for configuration.
- **Firewall settings** adjusted to allow sharing.

---

## 🛠️ Procedure and Steps to Follow

### 🔗 A. Network Configuration
1. Connect all computers to the same network (Wi-Fi or Ethernet).
2. Ensure each device has a unique IP address.
3. Enable Network Discovery:
   - Go to `Control Panel > Network and Sharing Center > Change advanced sharing settings`.
   - Turn on **Network Discovery** and **File and Printer Sharing**.

### 📁 B. Folder Sharing
1. Right-click the folder → Select **Properties**.
2. Go to the **Sharing** tab → Click **Advanced Sharing**.
3. Check **Share this folder** → Assign a **share name**.
4. Click **Permissions** → Set access levels (Read, Change, Full Control).
5. Apply and close.

### 🖨️ C. Printer Sharing
1. Go to `Control Panel > Devices and Printers`.
2. Right-click the printer → Select **Printer Properties**.
3. Navigate to the **Sharing** tab → Check **Share this printer**.
4. Assign a **share name** → Apply settings.

### 📂 D. Accessing Shared Resources
1. On another computer, open **File Explorer**.
2. Type `\\ComputerName` or `\\IPaddress` in the address bar.
3. Browse and access shared folders or printers.

### 🔄 E. File Transfer
1. Copy files from the shared folder.
2. Paste them into the desired location on the local machine.

---
<img width="1934" height="2690" alt="image" src="https://github.com/user-attachments/assets/bdd07084-37b9-4351-9d24-9783296a4195" />

---
## ⚠️ Precautions
- Disable **password-protected sharing** if open access is needed.
- Use **strong passwords** and manage **user permissions** carefully.
- Keep **firewall and antivirus** updated.
- Avoid sharing system-critical folders like `C:\Windows`.

---

## ✅ Result
- Users can access shared folders and printers across the network.
- Files can be transferred seamlessly.
- Documents can be printed remotely.
- Overall, this setup improves collaboration and resource utilization.

