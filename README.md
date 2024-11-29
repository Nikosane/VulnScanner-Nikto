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

## Test Servers
These servers are explicitly provided for legal vulnerability testing:

### 1. DVWA (Damn Vulnerable Web Application)
URL: [http://testphp.vulnweb.com](http://testphp.vulnweb.com)

### 2. OWASP Juice Shop
URL: [https://juice-shop.herokuapp.com](https://juice-shop.herokuapp.com)

### 3. WebGoat
URL: [http://webgoat.herokuapp.com](http://webgoat.herokuapp.com)

### 4. Hack the Box Starting Point
URL: [https://www.hackthebox.com](https://www.hackthebox.com) (Requires registration.)

---

## Example: Scanning a Test Server
To scan the DVWA test server:
```bash
nikto -h http://testphp.vulnweb.com
```

### Output:
The results will display:
- Web server headers.
- Identified vulnerabilities (e.g., outdated software, dangerous files).
- Recommendations to mitigate the issues.

Save the output to a file:
```bash
nikto -h http://testphp.vulnweb.com -output report.txt
```

---

```plaintext
MIT License
Copyright (c) 2024 [Nikosane]
Permission is hereby granted, free of charge, to any person obtaining a copy...
```
