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
|CPU Socket	Holds the processor (CPU); connects it to the motherboard.|
|RAM Slots (DIMM)	Slots to install memory modules (RAM).|
|Chipset	Manages data flow between CPU, RAM, and peripherals (divided into Northbridge/Southbridge or SoC).|
|BIOS/UEFI Chip	Firmware that initializes hardware and starts the boot process.|
|Power Connectors	Connect motherboard to the power supply (usually 24-pin and 8-pin connectors).|
|Expansion Slots (PCIe)	For adding graphics cards, sound cards, Wi-Fi cards, etc.|
|Storage Connectors (SATA, M.2)	Connect hard drives and SSDs.|
|CMOS Battery	Powers the BIOS memory to retain system settings when powered off.|
|USB Headers	Connect USB ports on the front panel of the case.|
|Front Panel Connectors	For power button, reset button, LED indicators, etc.|
|Cooling Fan Headers	Connectors for CPU and case fans.|
|Audio and LAN Chips	Provide onboard sound and network connectivity.|
|I/O Ports (Back Panel)	Includes USB ports, audio jacks, HDMI/DisplayPort, Ethernet, etc.|

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
