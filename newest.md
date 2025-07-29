
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

---

## 🔑 Product Keys & Redemption

### POSA Key (Point of Sale Activation)
- 25-character alphanumeric (5x5)
- PIN behind the POSA card
- Used for **Redemption** only, not activation
- Redeem at: [office.com/setup](https://office.com/setup) or [microsoft.com/redeem](https://microsoft.com/redeem)

> Once redeemed, linked permanently to one MSA (Microsoft Account)

### Product Key (PK)
- Used for **Activation**
- Identifies license type, version, activation count
- Not used for redemption

### Supported Products for Redemption:
- Microsoft 365 Family, Personal
- Office 2019 H&S, Office 2019 H&B

### Tools:
- **KIT Tool** – Key Information Tool (check key status)

---

## 📋 DIA Checklist (Download, Install, Activate)

### Redemption
- Sign in to MSA
- Mode/place of purchase
- Product name
- Status of POSA Key:
  - Created – Invalid (retailer issue)
  - Active – Redeemable
  - Consumed – Already used under another MSA

### Download
- From genuine source or Store app
- OS version compatibility
- Disc space
- Internet connection
- Antivirus & Firewall
- Browser compatibility
- Windows 10 S – App permissions

### Installation
- First-time or reinstallation?
- Subscription or perpetual
- Same device?
- OS Compatibility:
  - Office 2010–2019: Win 7 SP1 and up
  - Mac: varies per version
- Office versions check (via `appwiz.cpl`)
- Trial version removal
- Admin user account
- Domain restrictions
- Windows Installer service – Running
- Windows Updates – Paused

### Activation
- Validate product: Subscription/Perpetual
- Use correct MSA
- OS activated
- Check for trials or multiple versions
- Disable antivirus & firewall
- Date & time settings

---

## 💻 Mac Troubleshooting (Office)

### Common Errors & Fixes

#### Error Code: `0x8A010101`
- Check MSA
- Ensure not trying to activate Office 2011
- Uninstall Office 2011
- Reinstall & sign in

#### Error Code: `0xD0001043`
- Server issue – Restart Mac & retry
- Use License Removal Tool
- Reinstall Office

#### Error Code: `0xD000001c`
- Invalid characters in Mac name  
  Fix via:
  ```
  Apple > System Preferences > Sharing > Change computer name
  ```

#### Activation Prompt After Activation
- Reset credentials:
  - Keychain > Delete Office identities cache
  - Run License Removal Tool
  - Restart Mac

---

## 📦 Install Office on Mac

1. Finder > Downloads > Open `Microsoft_Office_installer.pkg`
2. Follow the prompts: Continue > Agree > Install
3. Use admin password if prompted
4. Customize apps if needed

> If installer won't open: move to Desktop, hold `Control + Click`, and choose Open

---

## 🌐 Useful Links

- [Activate Office for Mac](https://support.microsoft.com))
- [Troubleshoot Mac Install Issues](https://support.microsoft.com/en-us/office/what-to-try-if-you-can-t-install-or-activate-office-for-mac)
---

## 📖 Common Interview Questions & Scenarios

1. **Activation after motherboard replacement** – Ask about license type (Retail or OEM), check digital entitlement
2. **BSOD after update** – Troubleshoot with Safe Mode, In-place upgrade
3. **No drives during installation** – Load storage drivers or diskpart clean
4. **MS Store/Apps not launching** – Reset MS Store, SFC/DISM
5. **Windows Update Services** – Windows Installer, Cryptography, BITS, Windows Update, Windows Time
6. **Update to latest Windows** – Check compatibility, free space, TPM, and Secure Boot
7. **No sound after update** – Check device manager > Roll back audio driver
8. **Clean installation from bootable** – Boot from USB > Custom Install
9. **Win 11 Minimum Requirements** – TPM 2.0, Secure Boot, 4GB RAM, 64GB Storage, 1GHz CPU
10. **Clean boot steps** – `msconfig` > Disable all startup services except Microsoft
11. **Uninstall & reinstall Office via CMD** – Use `cscript` for activation removal
12. **SLUI 4 usage** – For phone activation
13. **Location of old files after custom install** – `Windows.old`
14. **Open user page / program features** – `netplwiz`, `appwiz.cpl`
15. **Latest Windows version** – Check via `winver`
16. **Reinstall after In-Place** – Keeps apps and files
17. **In-place upgrade architecture limitation** – Can't switch from 32-bit to 64-bit
18. **Create new local account** – `netplwiz`
19. **Network reset command path** – `Settings > Network & Internet > Advanced settings > Reset`
20. **Enable hidden admin** – `net user administrator /active:yes`

---

## ✅ Summary: Key Commands

| Purpose               | Command                  |
|------------------------|--------------------------|
| Enable Admin           | `net user administrator /active:yes` |
| Reset Store            | `wsreset.exe`            |
| SFC Scan               | `sfc /scannow`           |
| System Info            | `msinfo32`               |
| DirectX Version        | `dxdiag`                 |
| View Windows Version   | `winver`                 |
| Uninstall Program      | `appwiz.cpl`             |
| Create User Account    | `netplwiz`               |
| Clean Boot             | `msconfig`               |
| Open Services          | `services.msc`           |

---
