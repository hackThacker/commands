
# Commands of kali linux and windows 🧰

- [Kali Linux Commands](#Kali-Linux-Commands)
- [Windows Commands](#Windows-Commands)

### Kali Linux Commands:

#### Basic Commands:

1. **ls**
   ```markdown
   List files and directories in the current folder.
   ```

2. **cd**
   ```markdown
   Change current directory.
   ```

3. **pwd**
   ```markdown
   Print the current working directory.
   ```

4. **mkdir**
   ```markdown
   Create a new directory.
   ```

## Create Directory Structure for Nepal

The following command creates a directory structure for Nepal, including provinces and wards. Each province has a unique number (1 to 7), and within province 3, there are 19 wards.

```
mkdir -p nepal && cd nepal && for i in {1..7}; do mkdir -p "province$i"; done && mkdir -p province3 && cd province3 && for j in {1..19}; do mkdir -p "ward$j"; done
```

- `mkdir -p nepal`: Creates the main "nepal" directory.
- `cd nepal`: Changes into the "nepal" directory.
- `for i in {1..7}; do mkdir -p "province$i"; done`: Uses a loop to create directories "province1" through "province7."
- `mkdir -p province3 && cd province3 && for j in {1..19}; do mkdir -p "ward$j"; done`: Creates "province3," changes into it, and uses a loop to create "ward1" through "ward19" within "province3."

```

5. **cp**
   ```markdown
   Copy files or directories.
   ```

6. **mv**
   ```markdown
   Move or rename files and directories.
   ```

7. **rm**
   ```markdown
   Remove or delete files and directories.
   ```

8. **cat**
   ```markdown
   Display the contents of a file.
   ```

9. **echo**
   ```markdown
   Display text on the terminal.
   ```

10. **chmod**
    ```markdown
    Change file permissions.
    ```

#### Intermediate Commands:

1. **ps**
   ```markdown
   Display information about active processes.
   ```

2. **top**
   ```markdown
   Display and update sorted information about processes.
   ```

3. **kill**
   ```markdown
   Terminate or send signals to processes.
   ```

4. **ifconfig**
   ```markdown
   Configure and display network interface parameters.
   ```

5. **ping**
   ```markdown
   Test network connectivity to a specific IP address.
   ```

6. **netstat**
   ```markdown
   Display network connections, routing tables, interface statistics.
   ```

7. **grep**
   ```markdown
   Search for a pattern in files.
   ```

8. **tar**
   ```markdown
   Create and extract tar archives.
   ```

9. **nano**
   ```markdown
   Text editor for the command line.
   ```

10. **wget**
    ```markdown
    Download files from the internet.
    ```

#### Advanced Commands:

1. **nmap**
   ```markdown
   Network Mapper - scan and discover network hosts.
   ```

2. **airmon-ng**
   ```markdown
   Enable or disable monitor mode on wireless interfaces.
   ```

3. **arpspoof**
   ```markdown
   Spoof ARP replies to redirect traffic on a local network.
   ```

4. **wireshark**
   ```markdown
   Network protocol analyzer.
   ```

5. **john**
   ```markdown
   Password cracker.
   ```

6. **hydra**
   ```markdown
   Password brute-force tool.
   ```

7. **iptables**
   ```markdown
   Configure and manage IP packet filter rules.
   ```

8. **tcpdump**
   ```markdown
   Dump traffic on a network.
   ```

9. **metasploit**
   ```markdown
   Penetration testing framework.
   ```

10. **snort**
    ```markdown
    Network intrusion detection and prevention system.
    ```

#### Professional Commands:

1. **gpg**
   ```markdown
   GNU Privacy Guard - encrypt and sign data.
   ```

2. **sqlmap**
   ```markdown
   Automated SQL injection and database takeover tool.
   ```

3. **aircrack-ng**
   ```markdown
   Wi-Fi security auditing suite.
   ```

4. **setoolkit**
   ```markdown
   Social Engineering Toolkit - manipulate people into performing actions.
   ```

5. **hashcat**
   ```markdown
   Advanced password recovery.
   ```

6. **volatility**
   ```markdown
   Memory forensics framework.
   ```

7. **docker**
   ```markdown
   Containerization platform.
   ```

8. **exploitdb**
   ```markdown
   Exploit database archive.
   ```

9. **autopsy**
   ```markdown
   Digital forensics platform.
   ```

10. **mitmproxy**
    ```markdown
    Man-in-the-middle proxy for HTTP and HTTPS.
    ```

### Windows Commands:

#### Basic Commands:

1. **cd**
   ```markdown
   Change current directory.
   ```

2. **dir**
   ```markdown
   List files and directories in the current folder.
   ```

3. **echo**
   ```markdown
   Display text on the console.
   ```

4. **copy**
   ```markdown
   Copy files or directories.
   ```

5. **del**
   ```markdown
   Delete files.
   ```

6. **ipconfig**
   ```markdown
   Display IP configuration for all network interfaces.
   ```

7. **mkdir**
   ```markdown
   Create a new directory.
   ```
Certainly! Below is the command in Markdown format with a description:

```markdown
### Create Directories and Files in a Single Line

To create multiple directories and files in a single line using Command Prompt:

```
mkdir directory1\subdirectory1\subdirectory2 && echo Hello > directory1\subdirectory1\subdirectory2\file1.txt && echo World > directory1\subdirectory1\subdirectory2\file2.txt
```

#### Explanation:

- `mkdir directory1\subdirectory1\subdirectory2`: Creates the specified directory structure.
- `&&`: Executes the next command only if the preceding one succeeds.
- `echo Hello > directory1\subdirectory1\subdirectory2\file1.txt`: Creates a file named `file1.txt` and writes "Hello" to it.
- `echo World > directory1\subdirectory1\subdirectory2\file2.txt`: Creates a file named `file2.txt` and writes "World" to it.
```

## Create Directory Structure for Nepal

### Using Command Prompt (cmd)

The following command creates a directory structure for Nepal in Command Prompt, including provinces and wards. Each province has a unique number (1 to 7), and within province 3, there are 19 wards.

```batch
mkdir nepal
cd nepal
for /l %i in (1,1,7) do mkdir "province%i"
cd province3
for /l %j in (1,1,19) do mkdir "ward%j"
```
```
mkdir nepal && cd nepal && (for /l %i in (1,1,7) do mkdir "province%i") && (cd province3 && for /l %j in (1,1,19) do mkdir "ward%j")
```

- `mkdir nepal`: Creates the main "nepal" directory.
- `cd nepal`: Changes into the "nepal" directory.
- `for /l %i in (1,1,7) do mkdir "province%i"`: Uses a loop to create directories "province1" through "province7."
- `cd province3`: Changes into "province3."
- `for /l %j in (1,1,19) do mkdir "ward%j"`: Uses a loop to create "ward1" through "ward19" within "province3."

### Using PowerShell

The following command creates a directory structure for Nepal in PowerShell, including provinces and wards. Each province has a unique number (1 to 7), and within province 3, there are 19 wards.

```
New-Item -ItemType Directory -Path "nepal" -Force
Set-Location "nepal"
for ($i=1; $i -le 7; $i++) { New-Item -ItemType Directory -Name "province$i" -Force }
Set-Location "province3"
for ($j=1; $j -le 19; $j++) { New-Item -ItemType Directory -Name "ward$j" -Force }
```
```
New-Item -ItemType Directory -Path "nepal" -Force ; Set-Location "nepal" ; for ($i=1; $i -le 7; $i++) { New-Item -ItemType Directory -Name "province$i" -Force } ; Set-Location "province3" ; for ($j=1; $j -le 19; $j++) { New-Item -ItemType Directory -Name "ward$j" -Force }
```

- `New-Item -ItemType Directory -Path "nepal" -Force`: Creates the main "nepal" directory.
- `Set-Location "nepal"`: Changes into the "nepal" directory.
- `for ($i=1; $i -le 7; $i++) { New-Item -ItemType Directory -Name "province$i" -Force }`: Uses a loop to create directories "province1" through "province7."
- `Set-Location "province3"`: Changes into "province3."
- `for ($j=1; $j -le 19; $j++) { New-Item -ItemType Directory -Name "ward$j" -Force }`: Uses a loop to create "ward1" through "ward19" within "province3."

```

8. **ren**
   ```markdown
   Rename files or directories.
   ```

9. **type**
   ```markdown
   Display the contents of a text file.
   ```

10. **cls**
    ```markdown
    Clear the console screen.
    ```

#### Intermediate Commands:

1. **tasklist**
   ```markdown
   Display a list of running processes.
   ```

2. **netstat**
   ```markdown
   Display active network connections and listening ports.
   ```

3. **xcopy**
   ```markdown
   Copy files and directories with additional options.
   ```

4. **sfc**
   ```markdown
   System File Checker - scan and repair system files.
   ```

5. **chkdsk**
   ```markdown
   Check and repair disk errors.
   ```

6. **robocopy**
   ```markdown
   Robust file and folder copying with more options than copy.
   ```

7. **systeminfo**
   ```markdown
   Display detailed configuration information about the computer.
   ```

8. **ver**
   ```markdown
   Display the current Windows version.
   ```

9. **find**
   ```markdown
   Search for a specific string in files.
   ```

10. **regedit**
    ```markdown
    Registry Editor - modify Windows Registry settings.
    ```

#### Advanced Commands:

1. **gpupdate**
   ```markdown
   Force an immediate update of Group Policy.
   ```

2. **diskpart**
   ```markdown
   Disk Partitioner - manage disk partitions.
   ```

3. **pnputil**
   ```markdown
   Install or manage plug-and-play devices.
   ```

4. **schtasks**
   ```markdown
   Schedule tasks to run at specified times.
   ```

5. **wmic**
   ```markdown
   Windows Management Instrumentation Command-line - system information and configuration.
   ```

6. **bcdedit**
   ```markdown
   Boot Configuration Data Editor - configure boot options.
   ```

7. **netsh**
   ```markdown
   Network Shell - configure network settings.
   ```

8. **powercfg**
   ```markdown
   Power Configuration - configure power settings.
   ```

9. **cipher**
   ```markdown
   Encrypt or decrypt files and folders.
   ```

10. **dism**
    ```markdown
    Deployment Image Service and Management Tool - service and repair Windows images.
    ```

#### Professional Commands:

1. **ica

cls**
   ```markdown
   Display or modify Access Control Lists (ACLs) for files and folders.
   ```

2. **perfmon**
   ```markdown
   Performance Monitor - monitor and log system performance.
   ```

3. **gpresult**
   ```markdown
   Display Group Policy settings and applied policies.
   ```

4. **dcdiag**
   ```markdown
   Domain Controller Diagnostic Tool - diagnose domain controller issues.
   ```

5. **sc**
   ```markdown
   Service Control - manage services.
   ```

6. **auditpol**
   ```markdown
   Configure security auditing policies.
   ```

7. **taskkill**
   ```markdown
   Terminate or stop a running process or application.
   ```

8. **fsutil**
   ```markdown
   File System Utility - perform various file system operations.
   ```

9. **wevtutil**
   ```markdown
   Event Viewer Utility - manage event logs.
   ```

10. **takeown**
    ```markdown
    Take ownership of files or directories.
    ```