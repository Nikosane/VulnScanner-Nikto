# VulnScanner-Nikto



## Nikto: Web Server Scanning

## Description
Nikto is a web server scanner that tests web servers for dangerous files, outdated server versions, and potential vulnerabilities. This repository contains basic guidance on using Nikto for web server vulnerability assessment, along with test server recommendations.

---

## Installation
To install Nikto on a Linux-based system:

```bash
sudo apt update
sudo apt install nikto -y
```
Verify the installation:
```bash
nikto -Version
```

---

## Basic Usage
The basic command for scanning a target is:

```bash
nikto -h <target-ip or domain>
```

### Options
- `-h` : Specify the target hostname or IP.
- `-output` : Save the results to a file.
- `-Tuning` : Specify the type of tests to run (e.g., `x` for all).

Example:
```bash
nikto -h http://testphp.vulnweb.com -output report.txt
```

---
