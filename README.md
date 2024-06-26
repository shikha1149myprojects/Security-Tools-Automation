# Security Tools Automation

## Objective

The objective of this assessment is to conduct a comprehensive analysis of the server's security vulnerabilities, evaluate its current security posture, and provide actionable recommendations to enhance its security. Our aim is to ensure the server's protection against potential cyber threats.


### Skills Learned

- Programming: Writing and debugging code to automate security tasks using languages like Python, Java, or C++.
- Security Analysis: Identifying vulnerabilities and potential threats through automated scanning and monitoring.
- Tool Integration: Combining various security tools and APIs to create a comprehensive automated solution.
- Automation: Developing scripts and workflows to automate repetitive security processes and enhance efficiency.

### Tools Used

-Figlet: Generates stylized text banners in the terminal.

-Postfix: Mail transfer agent used for sending emails.

-Rustscan: Fast port scanner designed to quickly identify open ports on a target.

-Feroxbuster: Directory brute-forcing tool that scans for hidden directories and files on a web server.

-sendemail: Lightweight command-line email client.


### Steps

This project involves creating scripts to automate the installation of specific security tools and running scans on a target IP address. The main tasks are:

1. Installation Script (install_main.sh)
2. Scan Script (script_scan.sh)
   
Installation Script (install_main.sh)

Purpose:
To install necessary security tools (like figlet, postfix, nikto, rustscan, and feroxbuster) if they are not already installed on the system.

Process
1. Checks if each tool is installed.
2. If not, installs the tool.
3. Sets the correct permissions for the tools.
4. Prints confirmation messages to indicate the progress and completion of the installation.

   
Scan Script (script_scan.sh)

Purpose:
To perform a security scan on a given IP address, detect open ports, and send an email with the scan results.

Process
1. Takes an IP address as input.
2. Runs RustScan on the IP address to find open ports.
3. If port 80 (HTTP) is open, runs Feroxbuster to discover directories.
4. Saves the results in a file called results.txt.
5. Prompts the user for an email address and sends the results to this email.
