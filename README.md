# Nuclei Templates

A collection of custom security testing templates for [ProjectDiscovery Nuclei](https://github.com/projectdiscovery/nuclei).

## About

This repository contains a curated set of Nuclei templates designed to detect various security vulnerabilities, misconfigurations, and CVEs. These templates complement the official Nuclei template repository and provide additional coverage for specific vulnerabilities and attack vectors.

## Installation

To use these templates, simply copy them to your Nuclei templates directory:

### Default Installation Path

**Linux/macOS:**
```bash
~/.local/nuclei-templates/
```

**Windows:**
```
%USERPROFILE%\nuclei-templates\
```

### Quick Setup

1. Clone or download this repository
2. Copy the template files to your Nuclei templates directory:

```bash
# Linux/macOS
cp -r *.yaml ~/.local/nuclei-templates/

# Windows
copy *.yaml %USERPROFILE%\nuclei-templates\
```

## Usage

Once installed, you can use these templates with Nuclei:

```bash
# Run all templates from this repository
nuclei -t /path/to/templates -u https://target.com

# Run a specific template
nuclei -t /path/to/templates/CVE-2018-10383.yaml -u https://target.com

# Run templates with specific tags
nuclei -t /path/to/templates -u https://target.com -tags xss,cve
```

## License

This repository is provided for educational and security research purposes. Use responsibly and only on systems you own or have explicit permission to test.

## Disclaimer

These templates are provided as-is without any warranty. Users are responsible for ensuring they have proper authorization before testing any systems. The authors and contributors are not liable for any misuse or damage caused by these templates.

