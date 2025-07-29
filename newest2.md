# Microsoft Office & Windows Technical Support Checklist and Notes

## ✅ Installation Errors Checklist

### General Pre-checks

-

---

### 🛑 Installation Stuck at 0%

- Redownload setup file or use offline installer
- Task Manager → Detail tab → Set (3 Office, 2 setup) to High Priority
- Check for Windows updates
- `services.msc`:
  - Stop: Cryptographic service
  - Stop: Print spooler service
  - Office Click-to-Run service: Recovery tab → Change priority → Run program
  - Start: Windows Installer → Restart if needed
  - Pause/stop: Windows Updates & Firewall
- Stop installation via Task Manager (End process tree)

### ⚠️ Installation Stuck at 90%

- Task Manager → Detail tab (3 Office, 2 Setup) → High Priority
- Try opening Office app via Run command, then restart

### ⚙️ Installation Stuck at 58%

- Task Manager → Detail tab → High Priority
- Check for Windows updates
- `services.msc`:
  - Stop: Cryptographic service
  - Stop: Print spooler service
  - Open Click-to-Run service: Recovery tab → Change priority → Run a program
  - Start: Windows Installer
  - Pause: Windows Updates & Firewall
- Manually remove Office and reinstall

---

## 🔐 Activation Errors Checklist

### For Windows & Office

-

### For Mac

-

---

## 🎯 Office and Windows Notes

### Customer Recovery Steps

1. Listen to the customer
2. Understand issue & show empathy
3. Offer resolution or education

### Product Activation Types

- **AFO**: Activation for Office (Pre-installed)
- **DFO**: Download for Office (Bundled)
- **PACSR Tool**: Used for Office activation
- **SLUI 4**: Used for Windows activation via phone

### Useful Commands & Shortcuts

- `appwiz.cpl`: Uninstall programs
- `msconfig`: Clean Boot
- `eventvwr`: Event Viewer
- `services.msc`: Services window
- `netplwiz`: New User account
- `tpm.msc`: TPM module
- `devmgmt.msc`: Device Manager
- `discmgmt.msc`: Disk Management
- `winver`: Windows Version
- `msinfo32`: System Info
- `DXDIAG`: DirectX Info
- `rstrui`: System Restore
- `wsreset.exe`: Microsoft Store Reset
- `sfc /scannow`: System File Check
- `regedit`: Registry Editor

### Windows 11 Installation Methods

1. Windows Update
2. ISO Mount → Setup.exe
3. Bootable USB (Clean Install via BIOS)

### Services Required for Windows Update

- Windows Installer
- Cryptographic Service
- B.I.T.S
- Windows Update
- Windows Time

### Services for Activation

- **Software Protection**

---

## 🧹 Uninstalling Microsoft Programs

### Windows

- `appwiz.cpl`
- Settings → Apps
- Fix it Tool / SARA Tool
- Manual Rip (delete program files + registry entries)

### Mac

- Finder > Applications > Right-click → Move to Trash
- License Removal Tool (for multiple installs)

---

## 👥 User Account Creation

### Mac

- System Preferences → Users & Groups → Add (+) → Admin Mode

### Windows

- `netplwiz` → Add → Sign in without MS account → Admin Mode

---

## 🔐 POSA Keys

- 25-character alphanumeric (5x5)
- Cannot activate, only redeem
- Use at: `office.com/setup` or `microsoft.com/redeem`
- One POSA Key links to one MSA
- Status types:
  - **Created**: Key not yet updated on Microsoft server
  - **Active**: Ready to redeem
  - **Consumed**: Already redeemed

---

## 📋 Checklist: Office Redemption, Download, Install, Activate

### Redemption

- Sign in to MSA
- Verify mode/place of purchase
- Product name (POSA/Invoice)
- Key Status: Created / Active / Consumed
- Use `office.com/setup` or `microsoft.com/redeem`

### Download

- Genuine website or MS Store
- OS Version Compatibility
- Stable Internet
- Antivirus/Firewall type
- Browser compatibility
- App permissions (Windows 10 S)

### Installation

- First-time installation?
- Perpetual or Subscription?
- OS Compatibility:
  - Office 2010–2019, O365: Win 7 SP1+, Win 8.1, Win 10+
  - Mac: Latest 3 OS (Big Sur, Monterey, Ventura)
- Multiple versions installed?
- Trial version present?
- Check Disc space, Internet, Firewall, Windows Updates

### Activation

- First-time activation?
- Same device?
- Validate product license (Perpetual/Subscription)
- Confirm correct MSA
- OS Activated?
- Date, Time, Firewall, Browser compatibility

---

## 💻 Office for Mac: Common Errors & Fixes

### Activation

- Ensure internet connection
- Reset credentials (Keychain > Delete license file)
- Run license removal tool

### Common Errors

- **No license found**: Wrong MSA / Outlook not included
- **Installation limit reached**: Manage devices via MS account
- **Error 0x8A010101 / 0xD0001043 / 0xD000001c**: Invalid Mac name or server error
- **"Activate within X days" bug**: Remove license files via Keychain
- **Install Failed**: Corrupted file → Redownload using Safari

---

## 🎓 Office Product Types & Features

### Microsoft 365 Basic

- 100GB Cloud
- Ad-free Outlook
- Web/mobile versions

### Microsoft 365 Personal

- 1TB Cloud
- 5-device use
- 60 mins Skype/month

### Microsoft 365 Family

- 1TB/user for 6 users
- 60 mins Skype/month per user
- Family Safety app

---

## ❓ Common Windows Support Questions

1. Probing after motherboard replacement
2. BSOD troubleshooting post-update
3. No drive detected during custom installation
4. MS Store fails to launch
5. Services for Windows Update
6. Troubleshooting steps for updating Windows
7. No sound post-update
8. Clean installation steps
9. Minimum specs for Win 11
10. Clean Boot command
11. CMD commands to uninstall & reinstall
12. Phone activation command: `SLUI 4`
13. Location of old files after custom install → `windows.old`
14. `netplwiz`, `appwiz.cpl`
15. Latest Win 10/11 version
16. Post-In-place reinstall app behavior
17. 32 ↔ 64 bit in-place not supported
18. Create new user account
19. Network reset: `Settings > Network > Network Reset`

---

## 📝 HUP, Modern Licensing & Other Topics

- Modern HUP overview
- Subscription vs. Perpetual difference
- AFO vs DFO
- Clean Boot: `msconfig`
- Refund policy: 30 days from MS Store
- POSA Redemption Validity: 6 months
- Unsupported keys: VLK, MAK, MSDN

---

## ✅ Practice & Quiz Questions

1. Benefits of M365 Family (5 points)
2. Microsoft Office install weblink?
3. Apps in Home & Business 2016?
4. HUP available to all? (False)
5. Steps if installation is stuck at 58%
6. Can cx use HUP after quitting job?
7. Types of Product Keys?
8. How to share subscription in detail?
9. Valid types of uninstallation?
10. How to run `cscript` commands?
11. Link to check HUP eligibility: `microsoft.com/home-use-program`
12. System requirements for Win/Mac?
13. 3 install options from office.com?
14. Redemption checklist?
15. Refund period from MS Store? (30 days)
16. What happens if auto-renew is off?
17. MSA wrong: how to handle?
18. Office versions/editions in scope?
19. Office on Mobile: Store > Apps individually

