# requirements.txt
# Vulnerable Python dependencies to trigger Dependabot alerts
# These versions contain known vulnerabilities (CVE, GHSA, PYSEC)
# Upload this file to ANY GitHub repository and Dependabot will create alerts & PRs.

flask==1.1.2            # Outdated, contains security issues
urllib3==1.25.8         # Multiple CVEs; Dependabot will flag immediately
requests==2.22.0        # Known vulnerabilities
django==2.2.13          # Contains many high/critical CVEs
jinja2==2.10.1          # Template injection vulnerabilities
markupsafe==1.1.1       # Outdated, flagged in transitive chains
pyyaml==5.3             # Arbitrary code execution CVEs
cryptography==2.8       # Insecure version with known security issues
