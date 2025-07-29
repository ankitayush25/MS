# Microsoft Office & Windows Support Checklist

## ✅ Checklist for Installation Errors

- OS compatibility
- Internet connection (Wi-Fi/LAN) – disconnect other devices
- Trial version/another license – remove manually or use Fix It tool
- Hard disk capacity (storage)
- Setup file can be corrupted – redownload or use offline installer
- Antivirus – disable from system tray or use `Windows Firewall`/`services.msc`
- Windows updates running in background – pause via `services.msc`
- Hidden Admin account:  
  ```bash
  net user administrator /active:yes
  ```
- Clean boot / Safe mode
- Task Manager & Windows Services
- Disable Proxy settings
- User account – Admin
- Download Offline installer

### 🛠 If Installation is Stuck

#### Stuck at 0%
- Redownload setup or use offline installer
- Task Manager > Details > 3x Office + 2x Setup → Set High Priority
- Check Windows Updates
- `services.msc`:  
  - Cryptographic service → Stop  
  - Print Spooler → Stop  
  - Microsoft Office Click-to-Run → Recovery tab → Modify priority → Run a program  
  - Windows Installer → Restart  
  - Windows Update & Firewall → Stop/Pause  
- End installation process from Task Manager (Details tab)

#### Stuck at 90%
- Task Manager → Set priority (3 Office, 2 Setup)
- Try running Office apps from Run > Restart PC

#### Stuck at 58%
- Same steps as 0% with manual Office removal & reinstall

---

## ✅ Checklist for Activation Errors

- Correct Microsoft Account (MSA)
- Multiple versions installed – check via `cscript`
- Validate key (perpetual/subscription)
- OS compatibility and activation status
- Browser compatibility
- Disable antivirus or firewall
- Check proxy
- Update Office software
- Enable hidden admin:
  ```bash
  net user administrator /active:yes
  ```
- Network reset commands
- Change DNS:
  - `8.8.8.8`, `8.8.4.4`
  - or `4.2.2.2`, `4.2.2.1`

### On Mac:
- Office License Removal Tool
- Update Office
- Set correct Date & Time / Language
- Validate computer/user/drive names
- Remove & reinstall
- Create new user account

---

## 💬 Customer Handling Procedure

- Listen actively to identify dissatisfaction
- Assure empathy and support
- Provide resolution or educate if resolution isn't possible

---

## 🔧 Office Product Types

- **AFO** – Activation for Office (pre-installed)
- **DFO** – Download for Office (digital)

---

## ☎️ Phone Activation

### Office:
- Use PACSR tool (in RAVE)

### Windows:
- `Windows + R` → `SLUI 4`  
  Select country > Enter Installation ID > Get Confirmation ID

---

## 🧰 Windows Admin Tools

| Command         | Function                        |
|----------------|----------------------------------|
| `appwiz.cpl`    | Uninstall programs              |
| `msconfig`      | Clean boot                      |
| `eventvwr`      | Event Viewer                    |
| `services.msc`  | Windows Services                |
| `netplwiz`      | User Account Management         |
| `tpm.msc`       | TPM Settings                    |
| `devmgmt.msc`   | Device Manager                  |
| `discmgmt.msc`  | Disk Management                 |
| `winver`        | Windows version                 |
| `msinfo32`      | System Info                     |
| `DXDIAG`        | DirectX version                 |
| `rstrui`        | System Restore                  |
| `Wsreset.exe`   | Reset Microsoft Store           |

---

## 🔄 Windows 11 Upgrade from Windows 10

1. Check Windows Update in Settings
2. Custom Installation using ISO > Mount > Setup.exe
3. Clean Installation (Bootable Drive > BIOS Boot Priority)

> Use **MCT** (Media Creation Tool) to create bootable media

---

## 📌 TPM (Trusted Platform Module)

- Required for Windows 11
- TPM also supports Secure Boot & BitLocker encryption

---

## 🗃️ Windows.old

- Created during upgrade
- Can be used to roll back within 10 days (extendable to ~60 days once)

---

## 🧹 Uninstall Updates

- Settings > Windows Update > Update History > Uninstall Updates

---

## Required Services for Windows Update

- Windows Installer
- Cryptographic Service
- BITS (Background Intelligent Transfer Service)
- Windows Update
- Windows Time

---

## 🛠 Windows Activation

- `Software Protection` service

---

## Office Uninstallation

### Windows:
- `appwiz.cpl`, `Settings > Apps > Uninstall`
- FixIt Tool / SARA Tool / Manual Rip (`regedit`)

### Mac:
- Finder > Applications > Right Click > Move to Trash
- Use License Removal Tool for multiple installs

---

## 👤 User Account Creation

### Mac:
- System Preferences > Users & Groups > Add (+) > Admin

### Windows:
- `netplwiz` > Add > Sign in without Microsoft > Admin mode

---

## 🔐 Scratch Key Card

> If POSA key is scratched/damaged  
- Request proof of purchase (POP) + image of card with case number

---

## 🌍 Geo Blocking

> Key bought in one region, activated in another – may not work

---

## 🧭 Microsoft 365 Editions

| Edition     | Storage | Devices | Support         | Skype Minutes | Platforms     |
|-------------|---------|---------|------------------|----------------|----------------|
| Family      | 1TB/user| 6 users | Free Tech Support| 60/month       | All devices    |
| Personal    | 1TB     | 1 user  | Free Tech Support| 60/month       | All devices    |
| Basic       | 100GB   | 1 user  | Tech Support     | N/A            | Web/Mobile only|

---

## 🧩 Subscription vs Perpetual

| Type          | Key       | Sharing     | Updates     | Support          |
|---------------|-----------|-------------|-------------|------------------|
| Subscription  | Linked to MSA | Yes     | Auto Update | Tech Support     |
| Perpetual     | Product Key   | No      | Manual      | Limited Support  |

---

*(continued in the markdown file...)*  
