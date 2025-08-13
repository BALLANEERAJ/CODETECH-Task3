# CODETECH-Task3
codetech details
NAME : BALLA NEERAJ
Company : CODTECH IT SOLUTIONS
ID : CT08DH138
Domain: Data Analytics
Duration : june to August 2025
Mentor:  Neela Santosh Kumar

The provided Python script is a Modular Penetration Testing Toolkit designed as an educational and versatile tool for various penetration testing tasks. It is structured with modular components, each addressing a fundamental area of network and web security testing. Here's an overview of the project, its components, and functionality:

Purpose
The toolkit aims to facilitate network and application security assessments through automated scans and brute force attempts on systems you own or have explicit permission to test. It is geared toward learners and ethical hackers who want an integrated framework containing common penetration testing techniques.

Key Modules and Features
1. PortScanner
Performs TCP port scanning for a given target host.

Supports scanning a specific port, a range of ports with multithreading, or a predefined list of common ports.

Uses threading for efficient, concurrent scanning.

Reports discovered open ports with real-time logging.

2. BruteForcer
Supports brute force attacks on SSH services and HTTP login forms.

For SSH, tries username/password combinations using paramiko SSH client.

For HTTP, submits login POST requests and checks response status or page content for successful login indicators.

Can generate password combinations with customizable character sets and lengths.

3. NetworkMapper
Conducts ping sweeps over an IP subnet range to identify live hosts.

Uses concurrent pinging with subprocess calls adapting for Windows and Linux.

Logs responses with success or error messages per target IP.

4. VulnerabilityScanner
Performs basic vulnerability detection such as:

Checking SSH version banners against a list of known vulnerable versions.

Inspecting HTTP response headers for missing or insecure security headers (e.g., X-Frame-Options, HSTS).

Logs warnings and findings for discovered vulnerabilities.

5. PentestToolkit (Main Orchestrator)
Coordinates all modules and manages scan workflows.

Can run a full scan on a target that includes common port scanning and vulnerability checks for SSH and HTTP if respective ports are open.

Generates a summary report showing open ports, vulnerabilities found, and any credentials discovered via brute force.

User Interface & Usage
Command-line interface accepts arguments for:

Target host or IP.

Port range to scan.

Flags for launching SSH or HTTP brute force attacks.

Network ping sweep specification.

A full comprehensive scan that includes port scanning and vulnerability detection.

Shows color-coded and timestamped logs for info, success, warnings, and errors.

Allows flexible usage for targeted tests or full assessments.

Educational and Practical Highlights
Demonstrates fundamental penetration testing activities in Python.

Modular design facilitates extension and customization.

Uses concurrency for efficiency in network scanning.

Emphasizes ethical hacking principles with warnings for authorized use only.

Logs detailed output with color coding for readability.

Offers a practical toolkit for students, enthusiasts, and researchers starting with penetration testing on networks and services.

Summary
This project is a comprehensive, modular Python toolkit combining port scanning, brute forcing, network discovery, and vulnerability identification. Its design and implementation make it well-suited for educational purposes and basic security assessments, providing hands-on experience with key concepts and tools used by penetration testers.

If you want, I can guide you on how to run this toolkit effectively, help customize modules, or explain any part of the code in detail for your learning or academic research purposes.
