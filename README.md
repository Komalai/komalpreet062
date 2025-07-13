# Day - 1
**Date:** 25th June 2025

### Status:
I was absent today due to personal reasons.

### What I Missed:
The first session of Semester 3, which included an introductory training on Linux.

### Topics reportedly covered:
Basics of the Linux operating system
### Booting and it's types:
Booting is the process of starting or restarting a computer. In Linux, the booting process involves several stages that load the operating system and prepare the system for use.

**Types of booting:**
1. Cold Boot (Hard Boot)
Occurs when the computer is started from power off.

Complete hardware and software initialization.

Performed when the system is completely shut down and powered back on.

2. Warm Boot (Soft Boot)
Restarting the system without turning off the power.

Done by the reboot or shutdown command.

Faster than cold boot as it skips some hardware checks.
### Updates:

We are required to download and set up the following software for upcoming practicals:

**Oracle VirtualBox –** For running virtual machines

**Microsoft Visual C++ Redistributable –** Required for some system components

**Ubuntu 24.04.2 ISO –** To install and use Linux in a virtual environment
### Next Steps:

Download and install the above softwar
# Day-2
**Date:** 26th June 2025

Our professor tells us that after we finish our work, we should help our classmates. She says helping others is not only good for them, but also helps us learn better. When we explain something to a friend, we understand it more too.

# Introduction to linux:
### Kernel:
A kernel is the core component of an operating system. It is responsible for managing system resources and it acts as a bridge between hardware and software.
![WhatsApp Image 2025-06-26 at 20 58 25_248aabb5](https://github.com/user-attachments/assets/d135bbd1-3ba7-438d-bab0-9f1ed55930a9)

### Shell:
A shell is a program that acts as an interface between the user and the operating system kernel. It allows users to interact with the computer by typing commands.
Analogy: Chef & Waiter in a Restaurant
**Characters:**

 Chef → Kernel

 Waiter → Shell

 Customer → User
 
The shell is like a waiter who takes your order (command), and the kernel is like the chef who prepares the dish (executes the command). You never talk to the chef directly.To communicate with the chef we can communicate through the waiter only.

**Types of shell:**

1. Bash(Bourne Again Shell) - Most common and default shell
  
2. Sh (Bourne Shell) - Original shell
  
3. Zsh - Powerful and customizable.
  
4. Fish - Friendly interactive shell


**Further shell is divided ito two types:**

1. Command Line Shell:
  A command-line shell is a text-based interface where you type commands to tell the computer what to do, using a keyboard.

2. Graphical Shell:
A graphical shell is a user interface that lets you interact with the computer using pictures, icons, and menus, usually with a mouse.

# File System Structure:
### Directories:
### Root of everything: /
|   Directory   |   purpose   |
|---------------|-------------|
|/bin|Contains user executable files|
|/boot|Stores boot files needed to start (boot) the system|
|/dev|Stores boot files needed to start (boot) the system|
|/media|Temporarily stores external devices|
|/mnt|Temporarily mounted filesystems|
|/opt|Contains optional files|
|/usr|Contains user-related programs and files|
|/temp|Stores temporary files|
|/sbin|Contains system binary commands|

### Commands:

|   Command   |   Defination   |
|-------------|----------------|
|ls|Lists files and directories in the current folder.|
|whoami|Shows the current logged-in user’s name.|
|date|Shows the current date and time|
|cd|Changes the current directory|
|mkdir|Creates a new directory (folder)|
|cat|Displays the content of a file|
|touch|Creates a new empty file.|
|cp|Copies files or folders|
|pwd|Shows the current location/path|
|whereis|Shows the location of a command|
|whatis|Gives a brief description of a command|
|mv|Moves or renames files and directories|

the program we execute today :

![ubuntu-day2 1](https://github.com/user-attachments/assets/dc8548b1-6be9-4498-bcf0-5b72d6b8f99c)

![ubuntu-day2 2](https://github.com/user-attachments/assets/ba72d5c4-94a8-43a4-97ad-be93eb6ff9b6)

# Day - 3

In the third day of training,first we revise previous syllabus and then we proceed further.on third day we had viva of day -1 and day - 2.
### Permissions & Shell programming :

### File and directory permissions:

**chmod –** Change File Permissions

chmod stands for "change mode". It is used to change the permissions of a file or directory.

* chmod +x test.sh: Gives permission to run the script.
* chmod 444 test.sh: Changes file to read-only.

![read-only](https://github.com/user-attachments/assets/13af4914-f049-4dac-bbeb-7170ce1fea39)

![read-only_result](https://github.com/user-attachments/assets/891763d2-97eb-4698-82e3-52c5452a71b7)


# Redirection :

  In Linux, redirection means sending the input/output of commands to files or devices instead of the default screen  or keyboard .
  . Overwrite Redirection (For stdout): Redirects the standard output of a command to a file. If the file exists already contain script, it will be overwritten. ">" standard output.
  . Append Redirection (For stdout): Append the output to the file without compromising the existing data of the file.

# Assignment:
### Shell programming:
**Use of variables:**


![ubuntu missing5](https://github.com/user-attachments/assets/76e2def2-a3ef-4422-913c-88e6028a3faa)

![ubuntu missing4 1](https://github.com/user-attachments/assets/a606ddff-e0f5-4453-95d9-dc154e4b180d)

**Multiplication table of any number:**


![WhatsApp Image 2025-07-03 at 20 59 51_68994e28](https://github.com/user-attachments/assets/82850072-ee10-4f81-be96-63960a0f9aa6)


![table](https://github.com/user-attachments/assets/b94a8d17-57ac-4fbf-a7cd-7a466244c0a3)

**Comparing two variables:**

![image](https://github.com/user-attachments/assets/e76e03f5-ce3c-4cda-96a4-a1f86d112395)


![compare](https://github.com/user-attachments/assets/0fa465ce-2719-4282-bd4a-ed202734eb80)


# Day - 4

### File Compression :
File compression is the process of reducing the file size to save space or make transfer easier. Linux provides several built-in tools to compress and extract files and directories.

**Why Do We Compress Files?**
*To save space on your computer
*To send files faster (like in email or WhatsApp)
*To group many files into one (e.g., a ZIP file)

**Common Types of Compression**
*ZIP – Most common (like file.zip)
*RAR – Another type (like file.rar)
*TAR.GZ – Common on Linux systems

### gzip
Gzip, short for GNU Zip, is a command-line compression tool commonly found on Linux systems. It utilizes the Deflatecompression algorithm to reduce the size of files, making them more manageable for storage and transmission.

**Syntax**
gzip filename

### Wildcard	:
| Wildcard | Meaning | Example | Matches|
|----------|---------|---------|--------|
| * |	Matches zero or more characters |	ls *.txt |	a.txt, notes.txt, file123.txt |
| ? |	Matches exactly one character |	ls file?.txt |	file1.txt, fileA.txt (not file12.txt) |
| [ ] |	Matches one character from the set |	ls file[12].txt |	file1.txt, file2.txt |
| [a-z] |	Matches one character from a range |	ls file[a-c].txt |	filea.txt, fileb.txt, filec.txt |
| [! ] | Matches one character not in set	ls file | [!0-9].txt |	filea.txt, fileX.txt (not file1.txt) |
| { } |	Brace expansion for multiple patterns|	cp file{1,2,3}.txt /backup/|	file1.txt, file2.txt, file3.txt |

# Assignment :
### What are escape characters:

Escaping means protecting a character so the terminal doesn't give it a special meaning. Use backslash () for escaping.

|Escape Character|	Meaning|	Example|	Output|
|----------------|--------|--------|-------|
|\n|	New line|	echo -e "Hello\nWorld"|	Hello
World|
|\t|	Tab space|	echo -e "Hello\tWorld"|	Hello  World|
|\\|	Backslash (\)	|echo -e "C:\\Users"	|C:\Users|
|\"|	Double quote (")|	echo -e "\"Hello\""|	"Hello"|
|\'	|Single quote (')	|echo -e "It\'s fine"|	It's fine|
|\a|	Alert (bell sound)|	echo -e "\a"|	Makes a beep sound, if enabled|
|\b	|Backspace	|echo -e "Helloo\b"	|Hello|
|\r|	Carriage return (overwrite line)|	echo -e "123\rAB"|	AB3 (replaces beginning chars)|
*-e option in echo is used to enable interpretation of escape sequences.

### Quoting in linux:

|Quote |Type	|Symbol	|Purpose|
|------|-----|-------|-------|
|Single quotes|	' '|	Prevent all interpretation of special characters. Everything is taken literally.|
|Double quotes	|" "|	Allow variable and command substitution, but prevent word splitting and globbing.|

### Hardware:
Hardware refers to the physical parts of a computer system — the components you can see and touch. It includes everything from the keyboard and mouse to internal parts like the CPU and memory.

![WhatsApp Image 2025-06-30 at 11 37 51_d197f179](https://github.com/user-attachments/assets/81569b38-f25a-455b-ac7b-339e5711cb72)


**Components of Motherboard:**

|Component	|Function|
|----------|--------|
|CPU Socket|	Holds the processor (CPU); connects it to the motherboard.|
|RAM Slots (DIMM)|	Slots to install memory modules (RAM).|
|Chipset|	Manages data flow between CPU, RAM, and peripherals (divided into Northbridge/Southbridge or SoC).|
|BIOS/UEFI Chip|	Firmware that initializes hardware and starts the boot process.|
|Power Connectors|	Connect motherboard to the power supply (usually 24-pin and 8-pin connectors).|
|Expansion Slots (PCIe)|	For adding graphics cards, sound cards, Wi-Fi cards, etc.|
|Storage Connectors (SATA, M.2)|	Connect hard drives and SSDs.|
|CMOS Battery|	Powers the BIOS memory to retain system settings when powered off.|
|USB Headers|	Connect USB ports on the front panel of the case.|
|Front Panel| Connectors	For power button, reset button, LED indicators, etc.|
|Cooling Fan| Headers	Connectors for CPU and case fans.|
|Audio and LAN Chips|	Provide onboard sound and network connectivity.|
|I/O Ports (Back Panel)|	Includes USB ports, audio jacks, HDMI/DisplayPort, Ethernet, etc.|

**Various components of Hardware:**

|Category|	Description	|Examples|
|--------|-------------|--------|
| Input Devices|	Used to enter data into the computer|	Keyboard, Mouse, Scanner, Microphone, Webcam|
| Output Devices|	Used to display or output results from the computer|	Monitor, Printer, Speaker, Projector|
| Processing Unit|	Performs all calculations and tasks	CPU| (Central Processing Unit)|
| Storage Devices	|Used to store data permanently or temporarily|	Hard Drive (HDD), SSD, USB drive, CD/DVD|
| Communication Devices|	Used for data exchange between computers|	Modem, Network Interface Card (NIC), Router|

### Motherboard:

The motherboard is the main printed circuit board (PCB) in a computer or electronic device. It serves as the central backbone that connects and allows communication between all hardware components such as the CPU, memory (RAM), storage devices, power supply, and peripherals.

![WhatsApp Image 2025-06-30 at 11 37 51_45b351ad](https://github.com/user-attachments/assets/fa80b436-2c34-4f82-8651-92508115898b)


 **1. Basic Computer Architecture :**
 
|Term	|Definition|
|-----|----------|
|PC |(Hardware)	Physical components of a computer.|
|System Software|	OS installed on hardware (e.g., Windows, Ubuntu).|
|Application Software|	Installed on OS (e.g., MS Word, Chrome, VLC).|

**2. CPU & Internal Components :**

|Component	|Definition|
|----------|----------|
|CPU|	Central Processing Unit; brain of the computer.|
|Motherboard|	Main circuit board connecting all components.|
|RAM|	Volatile memory; data lost on shutdown.|
|ROM|	Non-volatile memory; stores firmware.|
|Cache|	Very fast memory between CPU and RAM.|
|Registers|	Small, fast memory inside CPU for temporary data.|
|Control Unit (CU)|	Directs data flow and operations in CPU.|
|ALU|	Performs calculations and logic.|
|Clock|	Synchronizes CPU operations using electrical pulses.|
|Transistors|	Basic switching units used in processing.|
|Chipset|	Controls communication; Northbridge and Southbridge.|
|CPU Socket|	Slot where CPU is mounted; fan usually above it.|

### 3. Storage Devices :

|Component|	Definition|
|---------|-----------|
|Hard Disk| (HDD/SSD)	Permanent storage for OS, apps, and files.|
|RAM|	Temporary, fast memory used during system operation.|
|Cache|	Small, faster memory for urgent data access.|
|Floppy| Disk	Old magnetic storage medium (now obsolete).|
|CD/DVD	|Optical media used to read/write data.|
|BD (Blu-ray Disk)|	High-capacity optical disk for HD media and backups.|

### 4. Power & Booting :

|Component	|Definition|
|----------|----------|
|Power Supply (SMPS)|	Converts AC to DC; supplies power to components.|
|UPS|	Battery backup for power outages.|
|CMOS| Battery	Maintains BIOS settings and system time.|
|Boot| Process	Power on → ROM → Bootstrap Loader → OS loads in RAM.|

### 5. Input/Output & Display:

|Component |Definition|
|----------|----------|
|Monitor|	Output device to display visuals.|
|HDMI Port|	High-definition video output for projectors/displays.|
|VGA Port|	Older analog video output; needs converter for HDMI.|
|Display| Adapter	Processes and displays graphics (GPU).|
|TV Tuner| Adapter	Enables TV signal input to PC.|

### 6. Networking & Communication :

|Component	|Definition|
|----------|----------|
|LAN (Local Area Network)|	Network connecting nearby computers.|
|Modem|	Converts digital ↔ analog signals for internet.|
|LAN Card / NIC|	Allows PC to connect to network via cable.|

### 7. Other Components & Concepts :

|Component |Definition|
|----------|----------|
|Drivers|	Software that lets OS interact with hardware.|
|BIOS Chip|	Firmware chip that starts hardware and loads OS.|
|Peripheral Devices|	External devices like mouse, keyboard, printer, etc.|
|PCI Slots|	Expansion slots for adding cards (e.g., sound, LAN).|
|Expansion Slots|	Slots for adding extra hardware (graphics, TV cards).|
|SATA Ports|	Connect HDDs and SSDs to motherboard.|
|Beep Sound|	POST error codes (e.g., via speaker/copper coil).|
|Cooling System|	Fans or heat sinks to prevent overheating.|
|Configuration|	System specs: RAM, CPU speed, storage, brand, e|

# Day - 5

### What is HDD?
HDD (Hard Disk Drive) is a non-volatile storage device that stores and retrieves digital data using magnetic storage. It contains spinning disks (platters) and read/write heads.

**Key Features**
* Long-term data storage
* Uses magnetic platters and mechanical arms
* Slower than SSDs
* Large storage capacity at low cost

 **Types of HDD**
|Type	|Description|
|-----|-----------|
|PATA (IDE)|	Older standard, slow, now obsolete|
|SATA	|Common in modern desktops/laptops|
|SCSI	|Used in servers, supports multiple devices, high performance|
|SSHD	|Hybrid: SSD speed + HDD capacity|
|External HDD|	Portable, connects via USB|
|Enterprise HDD|	For servers/data centers, 24/7 operation|

**HDD Form Factors**
|Form Factor|	Usage|
|-----------|------|
|3.5 inch|	Desktop computers|
|2.5 inch|	Laptops, compact PCs|

GPU (Graphics Processing Unit)
A specialized processor for rendering images, videos, animations, and visual content.

### What Causes GPU Failure?
|Cause|	Description|
|-----|------------|
|Overheating|	Dust, fan failure, poor airflow|
|Power| Surges	Electric surges or unstable PSU|
|Driver Conflicts|	Corrupt or outdated drivers|
|Physical Damage	|Dropping or improper handling|
|Age/Wear|	Heavy use over time causes degradation|

**What to Do When GPU Fails:**

|Step|	Action|
|----|-------|
|Check Connections|	Reseat the GPU and check cables.|
|Clean the Card|	Remove dust, check fans.|
|Switch to Integrated Graphics|	Remove the GPU and boot using onboard graphics to isolate the issue.|
|Try GPU on Another PC|	To confirm if the GPU is really faulty.|
|Stress Test|	Use software like FurMark or GPU-Z (if it still works) to monitor GPU performance and temperature.|
|Reinstall Drivers|	Use DDU (Display Driver Uninstaller) and reinstall clean drivers.|
|Check Temperature|	Ensure GPU isn’t overheating. Use tools like MSI Afterburner.|

**If GPU is dead:**

*If under warranty: Contact manufacturer
*If not: Replacement is recommended unless minor (e.g., fan) issue

### PSU (Power Supply Unit):

**Symptoms of PSU Issues:**
* PC won’t power on
* Random shutdowns or reboots
* Burning smell or electrical noise
* Flickering lights or fans
* 
### Diagnosis Steps:

|Method	|How To Do It|
|-------|------------|
|Check Power Cable/Outlet|	Test with a known working outlet and cable.|
|Paperclip Test (for ATX PSU)|	Short green and black wires on 24-pin connector to check if PSU turns on (fans spin). Be careful.|
|Test with Multimeter|	Check voltage output of 12V, 5V, and 3.3V rails.|
|Try Another PSU|	Swap with a known good PSU to confirm failure.|

**Safety Tips:**

* Always turn off and unplug the PC before opening the case.
* Ground yourself to avoid static damage.
* Don’t attempt PSU repairs unless you're trained — dangerous voltages are involved.

### PC Running Slow – Causes & Fixes

|Issue	|Explanation|	Fix/Solution|
|------|-----------|-------------|
|Too Many Startup Apps|	Slows boot time	Ctrl + Shift + Esc → Startup → Disable unnecessary apps|
|Low RAM|	Can’t multitask well	Upgrade RAM to 8GB+|
|Fragmented HDD|	File access delays (HDD only)|	Run Disk Defragmenter|
|Old/Faulty HDD|	Degrading speed|	Replace with SSD|
|Background Processes|	Resource hogging apps	|End unnecessary processes from Task Manager|
|Virus/Malware|	System lag & damage	|Scan with antivirus|
|Outdated Drivers	|Causes lag or crashes|	Update from Device Manager or manufacturer site|
|Overheating	Thermal| throttling slows system|	Clean fans, apply thermal paste|
|Too Many Browser Tabs|	High RAM usage	|Close tabs, use light browsers|
|Background Updates|	Slows performance|	Let updates finish or pause|
|Weak CPU|	Can’t handle new apps|	Upgrade processor (if possible)|

### Common Printer Problems & Solutions:

|Issue|	Cause|	Solution|
|-----|------|---------|
|Not Printing|	Loose cable / offline / driver|	Check connections; update driver|
|Printer Offline|	Manual setting or network issue|	Set printer online in settings|
|Paper Jam	|Misaligned or stuck paper	|Carefully remove paper & debris|
|Low Ink|	Empty or clogged cartridge	|Replace/refill cartridge; clean printhead|
|Poor Print Quality|	Dirty nozzle / wrong settings	|Run nozzle cleaning tool|


### BSOD (Blue Screen of Death):
BSOD is a critical Windows error screen caused by system crashes.

**What Causes BSOD?**

|Cause|	Explanation|
|-----|------------|
|Faulty Drivers|	Incompatible or corrupt|
|Hardware Failure|	RAM, GPU, HDD issues|
|Corrupt System| Files	Damaged Windows components|
|Malware	|Can corrupt system processes|
|Update Issues|	Failed or incomplete Windows updates|
|Overclocking/BIOS|	Unstable configuration|

 ### Crash Analysis Tools:
 
* Event Viewer – View system logs
* WinDbg – Analyze crash dump files
* 
  ### BIOS/UEFI & POST:

|Term|	Description|
|----|------------|
|BIOS|	Traditional firmware for booting|
|UEFI|	Modern firmware with faster boot, graphical UI, mouse support|

 ### Common BIOS Settings:
 
|Setting	|Description|
|Boot Order|	Choose drive to boot from|
|Secure Boot|	Protects against unauthorized OS|
|XMP Profile	|Enables RAM to run at full speed|
|Fan Control|	Adjust fan speed|
|Virtualization|	Enables VM support|
|SATA Mode|	Switch between AHCI/IDE for SSDs/HDDs|

### What is POST?
POST = Power-On Self-Test
It checks hardware before booting OS.

**Common POST Errors:**
|Error|	Cause|	Fix|
|-----|------|----|
|No Display / Beeps|	RAM not detected|	Reseat or change RAM|
|Continuous Beeps|	GPU or CPU issue	|Recheck installation or replace|
|No Beep / No Boot|	PSU or motherboard failure|	Test with another PSU|
|CMOS Error|	Dead CMOS battery|	Replace battery (CR2032)|
|Boot Device Missing|	Drive not found|	Reconnect drive, check boot order|
|Overclock Failed|	Unsafe BIOS settings|	Reset BIOS to default|

### Accessing and Resetting BIOS:
|Action	|Steps|
|-------|-----|
|Access BIOS|	Press Del, F2, or Esc during startup|
|Reset BIOS|	Select “Load Setup Defaults” or remove CMOS battery|
|Update BIOS|	Download from motherboard website|

# Day - 6
# Safe Mode
Safe Mode is a diagnostic mode in an operating system that starts the system with only essential files and drivers. It helps in fixing problems like software errors, driver conflicts, or malware.

### Types :

**1. Safe Mode –** Starts with basic drivers only.

**2. Safe Mode with Networking –** Includes internet/network drivers.

**3. Safe Mode with Command Prompt –** Opens Command Prompt instead of the normal desktop.

# Recovery Tools
Recovery tools are built-in or external tools used to troubleshoot, fix, or restore the system to a previous or working state.

### Types:

**System Restore –** Rolls back the system to a previous restore point.

**Startup Repair –** Fixes boot-related issues.

**Reset This PC –** Reinstalls Windows (with or without keeping files).

**Recovery Drive or Disk –** External drive used to access recovery options.

# OS Repair (Operating System Repair)
OS Repair refers to methods used to fix corrupted or missing system files without completely reinstalling the operating system.

Use repair commands:

sfc /scannow – Scans and restores system files.
DISM /Online /Cleanup-Image /RestoreHealth – Repairs corrupted Windows images.
Bootable USB for repair and system reinstall.

# Virus and Malware Symptoms

* Slow performance
* Frequent pop-ups
* Programs crashing
* Unknown apps installed
* Browser redirecting to strange websites

# Basic Virus/Malware Removal

**Using Safe Mode –** Run antivirus in safe environment.

**Using Antivirus Software –** Scan and delete threats.

**Using Malware Removal Tools –** Like Malwarebytes, AdwCleaner.

**Manual Removal –** Deleting infected files and apps.

**Resetting System –** Reinstall OS if damage is severe.

# Ways to back up Windows:

**1. File History -** Backs up personal files (Documents, Pictures, etc.) to an external drive automatically.

**2. Backup and Restore (Windows 7) -** Creates regular backups or a full system image. Still available in newer Windows versions.

**3. System Image Backup -** Makes a complete copy of your system, including OS and settings. Useful for full recovery.

**4. OneDrive (Cloud Backup) -** Backs up important folders (Desktop, Documents, Pictures) to the cloud.

**5. Manual Backup -** Copy important files manually to an external hard drive or USB.

**6. Third-Party Backup Tools -** Use software like Acronis, Macrium Reflect, or EaseUS for full or scheduled backups.

# RJ45 (Registered Jack 45) :
RJ45 is a standard connector used to connect computers and networking devices like routers and switches using Ethernet cables.

### Key Points about RJ45:

# How to Make a RJ‐45 Cable:
1. Strip the cable to remove 1 inch of the outer sheath.
2. Untwist and straighten the wires inside of the cable
3. Arrange the wires into the right order as following.

|Pin| Number	Wire Color (T568B)	|
|---|---------------------------|
|1|	White Orange	|
|2|	Orange	Transmit| 
|3|	White Green	Receive| 
|4|	Blue	Unused |
|5|	White Blue	Unused |
|6|	Green	Receive |
|7|	White Brown	Unused |
|8|	Brown|

![image](https://github.com/user-attachments/assets/08b500e9-2e5c-4696-9c11-00a7df39b5d0)

4. Trim the wires into an even line 1⁄2 inch (13 mm) from sheathing
5. Insert the wires into the RJ-45 connector.
6. Stick the connector into the crimping part of the tool and squeeze twice.
7. Remove the cable from the tool and check that all of the pins are down & test the cable.

# Day -7
# Networking  Basics
### Hosts :
A host refers to any device that connects to a network and is capable of sending or receiving data. This includes:

* Computers (Desktops, Laptops)

* Servers

* Smartphones

* Printers

* IP cameras

* IoT devices (like smart TVs, smart bulbs, etc.)

![host](https://github.com/user-attachments/assets/1beb5235-156d-475e-ac26-dc22f161f254)

# Network :
A network is a group of two or more connected devices (like computers, servers, or mobile phones) that are linked together to share resources, exchange data, and communicate with each other. These devices are connected using wired (like Ethernet cables) or wireless (like Wi-Fi) communication methods.

**Key Features:**
Data sharing (files, messages)

Resource sharing (printers, internet)

Communication (email, video calls)

Centralized or distributed control

# IP Address:
An IP address (Internet Protocol address) is a unique number assigned to each device connected to a network. It helps in identifying and locating devices so they can communicate with each other over the internet or a local network.

### Types of IP Addresses
**1. Public IP Address :** Assigned to your network by your Internet Service Provider (ISP), allowing devices within your network to communicate with the internet.

**2.Private IP Address :** Used within a private network (e.g., home or office) and not routable over the internet. Devices within the same local network communicate using private IPs.

### Properties of an IP Address:
**1. Unique**
* Every IP address must be unique within a network.

* This means no two devices on the same network can have the same IP address.

* If two devices have the same IP, it leads to IP address conflicts, and communication may fail.

* Example: If your laptop has the IP 192.168.1.10, no other device in that network can use the same address at the same time.

**2. Universal**
* IP addresses follow a universal standard that is understood worldwide.

* No matter where you are, IP addresses follow the same format (IPv4 or IPv6).

* This allows devices from different parts of the world to communicate with each other over the internet.

* It ensures global connectivity and compatibility between networks and devices.

### IPv4 (Internet Protocol Version 4):
**Address Length:**

* IPv4 uses a 32-bit address format.

* This means the IP address is made up of 32 binary digits (0s and 1s).

**Notation:**

* IPv4 addresses are written in decimal format.

* The 32 bits are divided into 4 groups, called octets.

* Each octet is separated by a dot (.).

* Each octet can range from 0 to 255.

* Example: 192.168.1.1.

**Address Space:**

* Since IPv4 uses 32 bits, it can have 2³² = 4,294,967,296 unique addresses.

* This gives approximately 4.3 billion possible IP addresses.

* Due to the large number of internet-connected devices, this space is becoming exhausted.

### IPv6 Explanation in Points
**Address Length:**

* IPv6 uses a 128-bit address format.

* This means each IP address is made up of 128 binary digits (0s and 1s).

* It provides a much larger range than IPv4.

**Notation:**

* IPv6 addresses are written in hexadecimal format.

* The 128 bits are divided into 8 groups, each containing 4 hexadecimal digits.

* Groups are separated by colons (:).

* Example: 2001:0db8:85a3:0000:0000:8a2e:0370:7334

**Address Space:**

* IPv6 provides 2¹²⁸ = 340 undecillion unique addresses.

* This is enough to assign trillions of addresses to every person or device on Earth.

* The huge space ensures scalability for the future internet.

### IPv4 vs IPv6:

|Feature|	IPv4|	IPv6|
|-------|-----|-----|
|Address Length|	32 bits (4 octets)|	128 bits (16 octets)|
|Address Format|	Decimal (e.g., 192.168.1.1)|	Hexadecimal (e.g., 2001:0db8::1)|
|Address Space|	~4.3 billion addresses|	~340 undecillion addresses|
|Configuration|	Manual or DHCP|	Auto-configuration (SLAAC) or DHCPv6|

![IP](https://github.com/user-attachments/assets/693b218c-c492-4a09-9aef-d6f8d4343d47)

# Notation:
### Binary Notation (used internally in networking)
* In binary notation, an IP address is written in binary (base-2) numbers — using only 0s and 1s.

* IPv4 addresses are made up of 32 bits, which are grouped into 4 sets of 8 bits (called octets).

* Computers use this format to understand and process IP addresses.

* Example:
Binary: 11000000.10101000.00000001.00000001
This represents the IP address in binary form.

### 2. Dotted Decimal Notation (used by humans)
* In dotted decimal notation, the 32-bit binary address is converted into 4 decimal numbers.

* Each 8-bit binary group (octet) is converted to a number between 0 and 255.

* The four decimal numbers are separated by dots (.).

* This is the standard readable format for IPv4 addresses.

* Example:
Binary:      11000000.10101000.00000001.00000001  
Decimal:     192      .168      .1        .1  
IPv4 Address: 192.168.1.1

# Classful Addressing in IP (IPv4)
Classful addressing is a system used in IPv4 to divide the IP address space into five classes (A to E) based on the first few bits of the IP address. Each class has a different range, size of network and host portions, and specific use.

This method helps in identifying how much of the IP address is used for the network part and how much is used for the host part.

### Structure of IPv4 Address:
* IPv4 address = 32 bits

* Divided into network part and host part (depending on the class)

**IP Address Classes:**  
|Class|	Starting Bits|	Range of First Octet|	Network/Host Bits	|No. of Hosts	Use|
|-----|--------------|---------------------|-------------------|----------------|
|A|	0xxxxxxx|	1 – 126|	8 bits (N) / 24 bits (H)|	~16 million per network	Large networks|
|B|	10xxxxxx|	128 – 191|	16 bits (N) / 16 bits (H)|	~65,000 per network	Medium-sized networks|
|C|	110xxxxx|	192 – 223|	24 bits (N) / 8 bits (H)|	254 hosts per network	Small networks|
|D|	1110xxxx|	224 – 239|	Not divided (multicast)|	Not for host addressing	Multicast communication|
|E|	1111xxxx|	240 – 255|	Reserved	Not used for devices|	Research & Experimental use|

 **Key Points of Classful Addressing:**
* Divides IP addresses into fixed classes (A–E).

* Helps in identifying the size of the network.

* Simple but wastes IP addresses (not efficient).

* Replaced by Classless Addressing (CIDR) for better IP utilization.

![462012671-628b0cc6-8c90-454d-bccd-ac12a5129733](https://github.com/user-attachments/assets/b3f6a8cc-aad9-4817-8579-827996df669d)

# Broadcast vs. Multicast vs. Unicast :

|Parameters|	Unicast|	Broadcast|	Multicast|
|----------|--------|----------|----------|
|Basics|	There is only one receiver and one sender.|	There are multiple receivers and one sender.|	There are multiple receivers and multiple senders.|
|Meaning and Definition|	Unicast is used to transfer data from a single sender to a single recipient.|	Broadcast sends data from one sender to all devices on a network.|	Multicast sends data from one or more senders to a selected group of receivers.|
|Mapping|	One-to-one type of communication.|	One-to-many type of communication.|	Many-to-many type of communication.|
|Uses|	Used for direct communication like web browsing, emails, etc.|	Used in TV/radio networks, ARP, DHCP discovery, etc.|	Used in stock exchanges, live video streaming, multimedia delivery.|

# Subnetting:
Subnetting is the process of dividing a large IP network into smaller, manageable sub-networks called subnets. It helps in efficient use of IP addresses, reduces network traffic, and improves security by isolating different parts of a network.
or 
Dividing a large network into smaller, more manageable sub-networks. It helps to utilize the network bandwidth in more intelligent way.

* Bandwidth: Capacity of network; data transmission rate (e.g., Mbps). Should be maximum.

* Latency: Delay in data transmission. Should be minimum.

* Host Bits: Denoted by '0's in subnet mask.

* Network IP: First IP of a subnet (cannot be assigned to host).

* Broadcast IP: Last IP of a subnet (cannot be assigned to host).

![image](https://github.com/user-attachments/assets/3dae5fc9-981f-4c78-b36a-b41a616dffcb)

### Subnet Mask :
A subnet mask is a 32-bit number used to separate the network part and the host part of an IP address. It helps identify which portion of the IP address refers to the network and which part refers to the host within that network.

* Example:
For IP 192.168.1.10 and subnet mask 255.255.255.0,

255.255.255.0 means the first 3 octets are the network part,

The last octet is for hosts.
### MAC (Media Access Control Address):

**Nature:** A unique, 12-character hexadecimal (alphanumeric) attribute used to identify individual electronic devices on a network.
Distinction from IP Address:
**MAC Address:** Identifies the physical location of a device within a local network. It's like your permanent home address. The manufacturer provides it.
**IP Address:** Signifies the device's global or internet-accessible identity. It's more like a temporary vacation rental address, changing depending on your network connection.

### DNS (Domain Name System):
It is a naming system for computers, service etc connected to the Internet or a private network. It translates domain names (www.google.com) into machine-readable IP addresses (172.217.160.142).

**Default Gateway:**
Its a device (typically a router) that acts as a pathway for data to leave a local network and reach other networks, including the internet.

### CIDR (Classless Inter-Domain Routing):
Modern method for IP allocation and routing, replacing classful addressing with more flexible network sizing (e.g., /24).
**Types of Cables**
**Twisted Pair:**
Types: Shielded (STP) and Unshielded (UTP).
Use: LANs (Ethernet).
**Coaxial:**
Use: TV networks, older computer networks.
**Fiber-Optic:**
Use: High-speed networks, long distances (most commonly used today).

# Numerical:

For 205.150.65.0/26. Find:
Subset mask
Number of subsets
Number of hosts
Network IP
Broadcast IP.

**Solution:**
1. Subnet Mask
/26 means 26 bits are used for the network portion.

So, the subnet mask in decimal is:

Copy
Edit
11111111.11111111.11111111.11000000 → 255.255.255.192
Subnet Mask = 255.255.255.192

2. Number of Subnets
Given: It's from Class C (default /24), and we're using /26

Subnet bits = 26 - 24 = 2 bits

Number of subnets = 2² = 4

Number of Subnets = 4

3. Number of Hosts per Subnet
Host bits = 32 - 26 = 6 bits

Number of hosts = 2⁶ - 2 = 64 - 2 = 62
(Subtract 2 for Network & Broadcast addresses)

Number of Hosts = 62 per subnet

4. Network IP (of first subnet)
Subnet range = 2⁶ = 64 IPs per subnet

First subnet starts at:

Network IP = 205.150.65.0

5. Broadcast IP (of first subnet)
Broadcast = Last IP of the subnet

First subnet = 205.150.65.0 – 205.150.65.63

Broadcast IP = 205.150.65.63

# Day-8
# What is DHCP?
DHCP stands for Dynamic Host Configuration Protocol.
It is a network protocol used to automatically assign IP addresses and other network configuration details (like subnet mask, gateway, DNS) to devices on a network.

### What does DHCP provide?
IP Address

Subnet Mask

Default Gateway

DNS Server addresses

Lease Time (how long the IP is valid)

### Real-life Examples of DHCP:
**Home Wi-Fi:**
When you connect your phone or laptop to your home Wi-Fi, it automatically gets an IP address. The Wi-Fi router acts as the DHCP server.

**Office Network:**
In a large company, a central DHCP server assigns IPs to hundreds of computers and printers automatically.

**Public Networks (Airports, Cafes):**
When you connect to public Wi-Fi, DHCP assigns your device a temporary IP.

### Without DHCP vs With DHCP
|Action|	Manual IP (No DHCP)|	DHCP (Automatic)|
|------|--------------------|-----------------|
|Set IP Address|	You do it manually|	Given automatically|
|Easy to Use?| No|	 Yes|
|Error chances|	High|	Low|

### Networking Commands: ping, traceroute, ifconfig

**1. ping Command**

**Purpose:**
To test if a device (usually a website or IP) is reachable on a network.

**How it works:**
Sends small data packets to a target IP/host and waits for a reply.

**Syntax:**
ping [hostname or IP address]

**Example:**
ping google.com

**Output Explanation:**
* Shows response time (in ms)

* Indicates if the destination is reachable

* If no reply, the host might be down or blocked
**In Linux**
<img width="1280" height="800" alt="ping" src="https://github.com/user-attachments/assets/2bcf9e76-0c83-4c94-ac46-168f34636efb" />
**In Window**
<img width="562" height="339" alt="image" src="https://github.com/user-attachments/assets/7c1fc472-39b0-4fe4-83b8-1bb3bb0a2fe2" />


### traceroute (Linux/macOS) / tracert (Windows)
**Purpose:**
To show the path (or route) that a packet takes to reach its destination.

**How it works:**
Displays all intermediate routers between your computer and the target.

**Syntax:**
traceroute [hostname or IP address]  # Linux/macOS
tracert [hostname or IP address]     # Windows

**Example:**
tracert google.com     # Windows
traceroute google.com  # Linux/macOS

**Output Explanation:**
* Shows each "hop" (router) the packet goes through

* Helps find slow or failing routers
**In Linux**
  <img width="1280" height="800" alt="traceroute" src="https://github.com/user-attachments/assets/3bd7061e-5b78-44bc-a80c-b2459295c970" />
**In Window**
  <img width="806" height="703" alt="image" src="https://github.com/user-attachments/assets/56497da4-6a6f-4cfe-9472-b86646e8be0b" />
  **Asterisks (*) in Traceroute – Meaning & Interpretation**
  **Meaning:**
Asterisks appear when the router does not respond within the time limit.
It shows a timeout for that attempt.

### ifconfig (Linux/macOS)
**Purpose:**
To view and configure the network interfaces (like Wi-Fi, Ethernet) on your device.

Note: On newer Linux systems, use ip a instead of ifconfig.

**Syntax:**
ifconfig
**Example Output:**
eth0: flags=4163<UP,BROADCAST,RUNNING> ...
        inet 192.168.1.5  netmask 255.255.255.0
**What it shows:**
IP address of each network interface

MAC address

Status (up/down)

Packets sent/received
  
### Ethernet:
It is used to connect devices with a physical cable so that they can communicate or access.

**How it Works:**
Plug one end of an Ethernet cable into your PC's network port.
Plug the other end of the cable into a modem or router.
Your PC can now communicate over the network and access the internet.
**Ethernet vs. Wi-Fi:**
|Feature|	Ethernet|	Wi-Fi|
|-------|---------|------|
|Signal|	Through cable (copper, fiber)	|Through air (radio waves)
|Speed|	faster|	Varies, can be slower than wired|
|Stability|	More stable|	Can be affected by walls, distance.|
|Security|	More secure|	Less secure|
|Mobility|	No (wired)	|Yes (moves freely)|

**Comparison of Network Types**
|Network Type|	Definition	Type|
|------------|----------------|
|Ethernet|	A specific wired technology for local area networking.|	LAN Technology (Wired)|
|Wi-Fi|	A specific wireless technology for local area networking.|	LAN Technology (Wireless)|
|LAN|	A network connecting devices within a limited area (e.g., home, office).|	Local Network|
|WAN|	A network that spans a large geographical area, often connecting multiple LANs.|	Wide Network|
|Internet|	A global system of interconnected networks using the Internet Protocol (IP) suite.|Global WAN|`

# Day-9
# Introduction to HTML:
**What is HTML?**
HTML stands for HyperText Markup Language.
It is the standard language used to create webpages and web applications.

HTML defines the structure of a webpage using elements called tags (like <h1>, <p>, <a>, etc.).

**Why is HTML important?**
Without HTML, web pages wouldn’t exist — it provides the skeleton of all websites.

It tells the browser what to display and how content is organized, such as:

Headings

Paragraphs

Links

Images

Tables

Forms

<img width="351" height="256" alt="image" src="https://github.com/user-attachments/assets/f979d3c6-a948-4453-8d90-edba8b35672b" />
**Output:**
<img width="278" height="162" alt="image" src="https://github.com/user-attachments/assets/d4ed2c4b-7be7-4fc0-a097-29bd9011d465" />

# Day-10
# Introduction to HTML & Web Basics
**What is the Web?**
The World Wide Web (WWW) is a system where information is shared and accessed over the Internet using websites. Websites are made using HTML, CSS, and JavaScript.

**What is HTML?**
HTML (HyperText Markup Language) is the foundation of every webpage.
**It is used to:**

Structure content (headings, paragraphs, lists, links, etc.)

Add elements like images, buttons, tables, and forms

Work alongside CSS (design) and JavaScript (functionality)
# Tag Breakdown:
|Tag|	Meaning|
|---|--------|
|<!DOCTYPE html>|	Tells browser it's an HTML5 document|
|<html>|	Root of the page|
|<head>|	Metadata, title, and links|
|<title>|	Title shown in the browser tab|
|<body>|	Content displayed on the page|

**Common HTML Tags**

|Tag|	Name|	Purpose & Example|
|---|-----|------------------|
|<h1> to <h6>|	Headings	|<h1>Main Title</h1> (largest to smallest)|
|<p>	|Paragraph|	<p>This is a paragraph.</p>|
|<a>|	Anchor (Link)|	<a href="https://google.com">Visit Google</a>|
|<img>|	Image|	<img src="image.jpg" alt="description">|
|<ul>, <ol>|	Unordered/Ordered List|	<ul><li>Item</li></ul>|
|<table>|	Table|	Used for rows and columns|
|<form>|	Form|	For user input (textboxes, buttons)|
|<br>|	Line Break|	Inserts a new line|
|<hr>|	Horizontal Rule|	Adds a horizontal line|
|<div>|	Division	|Used to group content (block element)|
|<span>|	Inline Container|	Used to style small inline content|

# Day-11

# Common Input Types

HTML input fields are created using the <input> tag.

|Input Type	|Purpose|	Example Code|
|-----------|-------|-------------|
|text|	Single-line text input|	<input type="text" name="username">|
|password|	Hides typed characters|	<input type="password" name="pass">|
|email|	Accepts only email format	|<input type="email" name="email">|
|number|	Numeric input only	|<input type="number" name="age">|
|date|	Date picker	|<input type="date" name="dob">|
|radio|	Choose one option from a group|	<input type="radio" name="gender">|
|checkbox|	Multiple selections	|<input type="checkbox" name="hobby">|
|submit|	Button to submit form	|<input type="submit" value="Submit">|
|reset|	Clears all inputs	|<input type="reset">|
|file|	Upload file	|<input type="file" name="upload">|
|tel|	Telephone number input	|<input type="tel" name="phone">|
|url| Website address	|<input type="url" name="website">|
|color|	Pick a color	|<input type="color" name="favcolor">|
|range|	Slider control	|<input type="range" min="1" max="10">|

# Example of HTML Form:

<img width="558" height="361" alt="image" src="https://github.com/user-attachments/assets/a6ce9721-35d6-480a-86ba-b80e6f3c5441" />
<img width="360" height="238" alt="image" src="https://github.com/user-attachments/assets/1d14d364-778c-4a3d-8d4f-0fb460c231be" />

# Semantic HTML
Semantic HTML refers to the use of HTML5 tags that clearly describe the purpose and meaning of the content. It helps in accessibility, SEO, and code readability.
**Common Semantic Tags**
|Tag	|Purpose|
|----|-------|
|<header>|	Top section of page (logo, nav, title, etc.)|
|<footer>|	Bottom section of page (copyright, links)|
|<nav>|	Navigation links to other pages|
|<section>|	A thematic grouping of content|
|<article>|	Self-contained content (e.g., blog post, news item)|
# Example of Sementic HTML:
<img width="613" height="481" alt="image" src="https://github.com/user-attachments/assets/05bb47dc-0f15-49c5-bcac-2c6fb6970afc" />
<img width="444" height="323" alt="image" src="https://github.com/user-attachments/assets/c0059037-d33d-4613-ae8d-83a14415a66d" />


# Day-12
# CSS Styling: Inline, Internal & External
### What is CSS?
CSS stands for Cascading Style Sheets. It's a language that lets you control the visual appearance of HTML content — things like layout, colors, fonts, spacing, and more.

You can add CSS to your web page in three main ways:

### 1. Inline CSS
This method places the CSS directly inside an HTML tag using the style attribute.

It's best used for quick changes or testing small tweaks.

**Example:**

<p style="color: green; font-size: 18px;">This text is styled using inline CSS.</p>
### 2. Internal CSS
In this approach, the CSS code is written inside a <style> tag, which is placed within the <head> section of your HTML file.

It's useful when you're working on just one page and want all styles to stay within that same file.

**Example:**

<head>
  <style>
    body {
      background-color: #f0fff0;
      font-family: Arial;
    }
    h1 {
      color: darkgreen;
    }
  </style>
</head>

### 3. External CSS
This method keeps your CSS in a separate file (with a .css extension) and links it to your HTML page using the <link> tag.

It's the most organized and reusable method, especially when you're working on a multi-page website.

HTML File:

<head>
  <link rel="stylesheet" href="styles.css">
</head>
styles.css File:

css
Copy
Edit
body {
  background-color: #e6ffe6;
  font-family: Verdana;
}
h1 {
  color: seagreen;
  text-align: center;
}
# Quick Comparison
|Feature|	Inline CSS|	Internal CSS|	External CSS
|-------|-----------|-------------|------------|
|Where it's written|	Inside the HTML tag|	In <style> within <head>|	In a separate .css file|
|Applies to	|Just one element	|One full HTML page	|Multiple pages|
|Can be reused?| Not reusable| Somewhat reusable| Highly reusable|
|Best for|	Quick edits or testing|	Small projects or one-pagers|	Full websites or large projects|

# Day-13

# What is Git and Why Use Version Control?
Git is a distributed version control system used to track changes in source code during software development.It helps manage code across multiple versions, developers, and updates.

### Why Use Version Control?
1. Tracks Your Work
2. Collaboration Made Easy
3. Backup and Safety
4.  Branching and Experimenting
5.  Open Source and Free

### Git Architecture:
 ### 1. Repository (Repo)
A storage location where Git tracks all changes made to your files over time.

Can be:

Local – stored on your own computer

Remote – hosted on platforms like GitHub, GitLab, or Bitbucket

### 2. Working Tree (or Working Directory)
The actual files and folders you're working with on your system right now.

It reflects the current version of your project

You make your changes here before saving them permanently with Git

### 3. Index (Staging Area)
A middle layer where you place files before committing them to the repository.

You use git add to move changes here

It gives you control over what goes into the next commit

Think of it as a review area before saving

<img width="692" height="454" alt="image" src="https://github.com/user-attachments/assets/7ab5537f-2f02-4948-9554-6ec21210f08a" />


# How to Use Git (Using Command Line)
# Step 1: Create or Clone a Repository
First, get the repository link (usually ends with .git) from GitHub

Open Git Bash (or terminal)

Run this command to clone the repository:

Move into the project folder:
<img width="633" height="612" alt="image" src="https://github.com/user-attachments/assets/b9571563-31ad-4d93-a3bd-dafbbbd9350d" />
<img width="735" height="374" alt="image" src="https://github.com/user-attachments/assets/b3d3479d-d39e-4963-836b-482f314d47bc" />

(Optional) Check the files using ls

# Step 2: Check Git Status
Use this to see changes or file status:

If it says "Up to date", everything is in sync

# Step 3: Create and Edit a New File
Create a new HTML file:

Open and write your code in it:


Save the file after editing (in Nano, press Ctrl + O, then Enter, then Ctrl + X to exit)

# Step 4: Add the File to Staging Area
Stage the file for commit:

**Warning:**
If you see a message like:
**warning:** in the working copy of 'index.html', LF will be replaced by CRLF
→ It means Git will convert line endings to match Windows (CRLF). It's safe to ignore.

### Step 5: Commit Your Changes
Save your changes to the local repo with a message:

Set your name and email using:


Try committing again:

### Step 6: Push to Remote Repository
Send your changes to GitHub:

You may be asked to authorize Git Credential Manager

Click "Authorize git-ecosystem"

Enter your GitHub username and password or token

# Now Check Your Repo!
