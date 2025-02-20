
# Internal Attacks
- security breaches initiated by individuals within an organization, such as employees
# Active Directory Domain
- Microsoft service that manages identities and access in a Windows network environment. An **AD Domain** is a collection of objects (users, computers, printers) controlled by a Domain Controller (DC)

#  Linux treats everything as a file even usb, disks files and directories
- - **Regular Files (`-`)** – Text, binary, or executable files.
- **Directory (`d`)** – Container for files (`ls -l` shows `d` at the start).
- **Character Device (`c`)** – Terminals, USBs (`/dev/tty0`).
- **Block Device (`b`)** – Hard drives (`/dev/sda1`).
- **Symbolic Links (`l`)** – Shortcuts pointing to files.


# Usb USB auto-detection
- ### **How USB Devices Are Detected**
1. **Kernel detects the USB connection** (`dmesg` logs show device initialization).
2. **Device node is created** in `/dev/` (e.g., `/dev/sdb` for USB storage).
3. **Udev system assigns rules** and loads drivers (`/etc/udev/rules.d/`).
4. **Mounting the USB**
    - Manually: `sudo mount /dev/sdb1 /mnt/usb`
    - Automatically: `udisksctl mount -b /dev/sdb1`

# Zeek tool
- **network security monitoring tool** that analyzes network traffic and logs security-relevant data
# Snort Tool
- Detects suspicious network activity (DoS, buffer overflow, exploits).
# **OSSEC**
- Monitors system logs, file integrity, and user behavior.
# TCP VIEW
- **Green**: New connections made since you launched TCPView.
- **Red**: Closed connections.
- **White**: Ongoing connections.
![[20250123-2058-00.4105203.mp4]]



