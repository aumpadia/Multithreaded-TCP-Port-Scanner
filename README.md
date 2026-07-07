# Multithreaded TCP Port Scanner

A lightweight TCP port scanner built in Python using socket programming and multithreading.

The scanner checks a user-defined range of TCP ports, identifies common services running on open ports, performs basic banner grabbing, and displays scan statistics such as execution time and scan rate.

This project was developed to strengthen concepts related to Computer Networks, socket programming, and concurrent programming.

---

## Features

- Concurrent TCP port scanning using `ThreadPoolExecutor`
- Detects open TCP ports
- Identifies common services (HTTP, SSH, FTP, SMTP, etc.)
- Performs basic banner grabbing on open ports
- Resolves hostnames to IP addresses
- Displays scan progress in real time
- Shows scan statistics including execution time and ports scanned per second
- Built entirely using Python's standard library

---

## Technologies Used

- Python
- Socket Programming
- ThreadPoolExecutor
- TCP/IP Networking

---

## Project Workflow

```
User Input
     │
     ▼
Resolve Hostname
     │
     ▼
Create Port List
     │
     ▼
Concurrent Port Scan
     │
     ▼
Detect Open Ports
     │
     ▼
Banner Grabbing
     │
     ▼
Generate Scan Report
```

---

## How to Run

Clone the repository

```bash
git clone https://github.com/aumpadia/Multithreaded-TCP-Port-Scanner.git
```

Navigate to the project

```bash
cd Multithreaded-TCP-Port-Scanner
```

Run the program

```bash
python scanner.py
```

Enter:

- Target hostname or IP address
- Starting port
- Ending port

The program will scan the specified range and display all detected open ports along with service information.

---

## Example Output

```
============================================================
Custom Port Scanner
============================================================

Target : localhost

Scanning...

PORT      STATUS      SERVICE
--------------------------------
22        OPEN        SSH
80        OPEN        HTTP
443       OPEN        HTTPS

============================================================
Total Ports Scanned : 1024
Open Ports Found    : 3
Time Taken          : 2.84 seconds
Ports / Second      : 360.56
============================================================
```

---

## Networking Concepts Demonstrated

- TCP Socket Programming
- Client-Server Communication
- Port Scanning
- DNS Resolution
- Multithreading
- Banner Grabbing
- Network Service Identification

---

## Possible Improvements

Some future enhancements include:

- UDP port scanning
- IPv6 support
- Command-line arguments using `argparse`
- Export scan results to CSV or JSON
- Protocol-specific banner detection
- Scanning multiple hosts in a subnet

---

## Disclaimer

This project was developed for educational purposes.

Only scan systems that you own or have explicit permission to test.

---

## License

This project is licensed under the MIT License.
