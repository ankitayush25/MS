# Microsoft Office Support Guide

---

## Redemption & Activation

### What is Redemption?
- Redemption links your Office product key to a Microsoft Account (MSA).
- Once redeemed, it cannot be unlinked.

### Redemption Process:
1. **Create** an MSA (if not already existing).
2. **Activate** the key by redeeming it.
3. **Consume** the product by downloading and installing it.

### Where to Redeem:
- Visit: [setup.office.com](https://setup.office.com), [office.com/setup](https://office.com/setup), or [microsoft.com/redeem](https://microsoft.com/redeem)
- Sign in with MSA > Enter 25-digit key > Select language/country > Key binds permanently to MSA

### Redemption Compatibility:
- Redemption can be done on any device: PC, Mac, or Phone.
- Valid for both POSA keys and retail keys.
- Retail key flow: setup.office.com > Sign in > Enter key > Download > Use key to activate.

## Product Key

- 25-character alphanumeric (no A, E, I, O, U, 0, 8)
- Used to determine product license, version, edition, and activation status
- **Supported**: Retail, HUP
- **Unsupported**: VL, VLK, KMS, MAK, MSDN

### POSA Keys
- Point of Sale Activation
- Ends with "Z"
- PIN on the back of card
- Validity: 6 months from purchase
- Redemption URLs: setup.office.com/redeem, office.com/setup
- 1 POSA = 1 MSA
- Key Status:
  - **Created** – Not yet active, return to retailer
  - **Active** – Ready to redeem
  - **Consumed** – Already redeemed on another MSA

## Installation Methods

### 1. Click-to-Run (C2R)
- Go to [accounts.microsoft.com](https://accounts.microsoft.com) > Subscriptions > Install
- Quick install (2–3MB) that downloads and installs Office automatically

### 2. Microsoft Store
- Use Microsoft Store app for direct installation

### 3. Offline Installer
- From Subscriptions > Use small down-arrow near Install > Offline Installer

## Uninstallation Methods

1. Microsoft Support and Recovery Assistant (SaRAcmd)
2. Control Panel > Programs > Uninstall
3. Manual removal

## Troubleshooting Installation/Download Issues

### Basic Checklist:
1. Try another browser
2. Check disk space
3. Validate subscription
4. Note error codes
5. Ask how they’re installing
6. Remove any older Office versions (Control Panel or SaRAcmd)
7. Ask for OS version
8. Check antivirus and firewall

### Additional Probing:
- Product name
- Error message
- Use of VPN (geo-lock)
- Windows version
- Browser compatibility
- Windows 10 S Mode limitations

### Stuck Installation:
- **0%**: Retry with offline installer, stop conflicting services, end setup processes
- **50%**: End task from Task Manager, reboot, use SaRA tool
- **90%**: Set process to high priority in Task Manager
- Office apps open but setup stuck: Reboot and let setup finish

## Activation
- Sign into Word or any Office app > Go to Account > View activation status

## Family Subscription
1. Share via accounts.microsoft.com > Subscriptions > Share
2. Enter family member’s email
3. Recipient gets invitation to accept

## Troubleshooting Redemption Issues
- Key already used
- Key expired (older than 6 months)
- Server/network issues
- Retailer hasn’t activated key on Microsoft server
- Use Key Info Tool (KIT) - deprecated now

## Office Activation on Mac
- Use Microsoft License Removal Tool
- Check for updates
- Change DNS to 8.8.8.8
- Ensure correct time/date
- Avoid special characters in user/device names
- Reinstall if needed

## DIA (Download, Install, Activation) Checklist

### Basic Questions:
- Sign in to MSA?
- Mode of purchase: Retailer or Online?
- Product name (Invoice or POSA)?
- Key status: Created / Active / Consumed
- Key validity (under 6 months)?
- Correct redemption site?

### Download Troubleshooting:
- Source: Genuine website or Microsoft Store
- At what step is it stuck?
- OS version compatibility
- Disk space
- Internet stability
- Antivirus / Firewall checks

### Installation Troubleshooting:
- Is it first-time installation?
- Is it a perpetual license or subscription?
- Reinstalling due to updates, device change?
- Multiple Office versions installed?
- System admin access?
- Domain restrictions?
- Use hidden admin if needed
- Stop updates & firewall temporarily
- Stable Wi-Fi or LAN recommended

---

## Windows Activation Troubleshooting

### Checklist:
- Windows edition matches product key
- Internet connection is stable
- Run Activation Troubleshooter: Settings > Activation > Troubleshoot
- Use CMD:
  - `slmgr /dli`
  - `slmgr /xpr`
  - `slmgr /ipk <key>`
  - `slmgr /ato`
- If tied to digital license, sign into Microsoft Account
- If hardware was changed, use "I changed hardware" option

---

## Quick Repairs (If Office App Has Issues)
- Try Quick Repair and Online Repair via Control Panel > Programs > Office > Change

---

✅ End of Updated Support Document

