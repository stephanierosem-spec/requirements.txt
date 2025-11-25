# requirements.txt


flask==1.1.2            # Outdated, contains security issues
urllib3==1.25.8         # Multiple CVEs; Dependabot will flag immediately
requests==2.22.0        # Known vulnerabilities
django==2.2.13          # Contains many high/critical CVEs
jinja2==2.10.1          # Template injection vulnerabilities
markupsafe==1.1.1       # Outdated, flagged in transitive chains
pyyaml==5.3             # Arbitrary code execution CVEs
cryptography==2.8       # Insecure version with known security issues
version: 2
updates:
  - package-ecosystem: "pip"
    directory: "/"          # Look for requirements.txt in the repo root
    schedule:
      interval: "daily"     # Check for updates every day
