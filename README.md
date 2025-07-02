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

![Image](https://github.com/user-attachments/assets/b80c15ad-b914-4036-a116-7a3e00a4474d)

![Image](https://github.com/user-attachments/assets/a4551a32-08a8-4804-9a1d-62d8c1e7668e)

# Day - 3
**Date -** 25th June 2025

In the third day of training,first we revise previous syllabus and then we proceed further.on third day we had viva of day -1 and day - 2.
### Permissions & Shell programming :

### File and directory permissions:

**chmod –** Change File Permissions

chmod stands for "change mode". It is used to change the permissions of a file or directory.

* chmod +x test.sh: Gives permission to run the script.
* chmod 444 test.sh: Changes file to read-only.

# Redirection :

  In Linux, redirection means sending the input/output of commands to files or devices instead of the default screen  or keyboard .
  . Overwrite Redirection (For stdout): Redirects the standard output of a command to a file. If the file exists already contain script, it will be overwritten. ">" standard output.
  . Append Redirection (For stdout): Append the output to the file without compromising the existing data of the file.

# Day - 4
**Date -** 25th June 2025

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

