# Nmap Command Guide

This guide provides an overview of using the Nmap command line tool for network scanning and security auditing.

## Table of Contents
1. [Introduction](#introduction)
2. [Installation](#installation)
3. [Basic Usage](#basic-usage)
4. [Options and Parameters](#options-and-parameters)
5. [Examples](#examples)
6. [Best Practices](#best-practices)
7. [Resources](#resources)

## Introduction
Nmap (Network Mapper) is a powerful open-source tool used for network exploration and security auditing. It is designed to discover hosts and services on a computer network, thus creating a "map" of the network.

## Installation
Nmap is available for various operating systems including Windows, Linux, and macOS. 

- **Windows**: Download the installer from the [Nmap official website](https://nmap.org/download.html) and follow the installation instructions.
- **Linux**: Most Linux distributions have Nmap available in their package repositories. You can install it using the package manager (e.g., `sudo apt install nmap` for Debian/Ubuntu).
- **macOS**: You can install Nmap via Homebrew by running `brew install nmap`.

## Basic Usage
To perform a basic network scan using Nmap, you can use the following syntax:
Replace `[scan type]` with the type of scan you want to perform, `[options]` with any additional options you want to include, and `target` with the IP address or hostname of the target system.

## Options and Parameters
Nmap provides a wide range of options and parameters to customize your scans. Some common ones include:
- `-p`: Specifies the ports to scan.
- `-sV`: Enables version detection.
- `-O`: Enables OS detection.
- `-A`: Enables aggressive scanning options.
- `-T`: Specifies the timing template (speed) of the scan.

Refer to the [Nmap documentation](https://nmap.org/book/man.html) for a comprehensive list of options and parameters.

## Examples
Here are some practical examples of using Nmap:
- Scan a single host: `nmap 192.168.10.8`
- ![image](https://github.com/Umair86247/Nmap-Command-Guide/assets/160429176/3c0ccc21-3298-46f5-91a7-43628a115c45)
- Scan a range of IP addresses: `nmap 192.168.10.8-100`
- ![image](https://github.com/Umair86247/Nmap-Command-Guide/assets/160429176/2d5d6524-3316-49a1-984f-34761b41b040)
- Scan a specific port: `nmap -p 80 192.168.10.8`
- ![image](https://github.com/Umair86247/Nmap-Command-Guide/assets/160429176/c2b35435-a582-4dac-a1e1-aa5047ad4151)
- Perform an aggressive scan: `nmap -A 192.168.10.8`
- ![image](https://github.com/Umair86247/Nmap-Command-Guide/assets/160429176/2fb89966-569c-4fde-9950-81f53e709161)
- ![image](https://github.com/Umair86247/Nmap-Command-Guide/assets/160429176/010f96a2-fda5-4131-885e-413d50fc4dcc)
- ![image](https://github.com/Umair86247/Nmap-Command-Guide/assets/160429176/5d48438a-b873-4055-8a8a-5a39464f9ff8)
- ![image](https://github.com/Umair86247/Nmap-Command-Guide/assets/160429176/7e7048e8-965d-4fae-92aa-7e617550122c)
- ![image](https://github.com/Umair86247/Nmap-Command-Guide/assets/160429176/dc9d98fd-377d-4ab2-b1a1-b62713b667ed)
- Enables version detection: `nmap -sV 192.168.10.8`
- ![image](https://github.com/Umair86247/Nmap-Command-Guide/assets/160429176/8cd69d58-3dda-496b-b291-36c10dc7d25f)
- Increases verbosity level. Use multiple times for more verbosity: `nmap -v 192.168.10.8`
- ![image](https://github.com/Umair86247/Nmap-Command-Guide/assets/160429176/f5e94a34-018a-4112-9b92-1fc6055c8cf3)
- ![image](https://github.com/Umair86247/Nmap-Command-Guide/assets/160429176/d6f3d511-a231-4c36-bd43-3eca4f60c168)
- Runs a script against the target: `nmap -sV --script vulners 192.168.10.8`
- ![image](https://github.com/Umair86247/Nmap-Command-Guide/assets/160429176/d55f53fb-df96-4b76-a56e-164c4d69cf54)
- ![image](https://github.com/Umair86247/Nmap-Command-Guide/assets/160429176/ee71724b-83e1-4315-a685-76da834ce679)
- ![image](https://github.com/Umair86247/Nmap-Command-Guide/assets/160429176/1514b718-fb02-4a88-9311-e481a5fc9c18)
- ![image](https://github.com/Umair86247/Nmap-Command-Guide/assets/160429176/504b39d5-29c5-4da8-92ef-26820d670314)
- ![image](https://github.com/Umair86247/Nmap-Command-Guide/assets/160429176/b46ac241-2b31-461f-84ec-2ef7e931af51)
- ![image](https://github.com/Umair86247/Nmap-Command-Guide/assets/160429176/b2c1af26-b0cb-41ed-b583-b49ff8bde0b4)
- ![image](https://github.com/Umair86247/Nmap-Command-Guide/assets/160429176/d2b8dc4b-3b3f-4797-87df-bbc95e166747)
- ![image](https://github.com/Umair86247/Nmap-Command-Guide/assets/160429176/e83723ac-34d3-4788-a225-a06ef8d34d96)
- ![image](https://github.com/Umair86247/Nmap-Command-Guide/assets/160429176/80a62579-5b06-4369-90b9-2332171dd631)
- ![image](https://github.com/Umair86247/Nmap-Command-Guide/assets/160429176/0537803f-a5f8-4efc-8153-ac4053d628c5)
- ![image](https://github.com/Umair86247/Nmap-Command-Guide/assets/160429176/2b91abd6-4ed8-45a0-a6b4-6573813bf748)
- ![image](https://github.com/Umair86247/Nmap-Command-Guide/assets/160429176/b3ff10d4-bce6-4696-a25a-4948be49b1f1)
- ![image](https://github.com/Umair86247/Nmap-Command-Guide/assets/160429176/f2d14a2f-0004-4138-8b0c-67445aed01f0)
- ![image](https://github.com/Umair86247/Nmap-Command-Guide/assets/160429176/caf75124-5fec-4f99-a820-397d33e57273)
- ![image](https://github.com/Umair86247/Nmap-Command-Guide/assets/160429176/f3459da1-a8b7-4e38-b046-7a4a19c52612)
- ![image](https://github.com/Umair86247/Nmap-Command-Guide/assets/160429176/6408ef2f-0f64-4d54-9c3d-dfabf1e8d711)
- Enables OS detection: `nmap -O 192.168.10.8`
- ![image](https://github.com/Umair86247/Nmap-Command-Guide/assets/160429176/8a4dffc8-c54e-4284-82ca-eebf3f80c442)




## Best Practices
When using Nmap:
- Ensure you have proper authorization before scanning any network or system.
- Be cautious when performing aggressive scans as they can generate significant network traffic.
- Check the legality and terms of service before scanning external networks.

## Resources
- [Nmap Official Website](https://nmap.org/)
- [Nmap Reference Guide](https://nmap.org/book/man.html)
- [Nmap Wiki](https://en.wikipedia.org/wiki/Nmap)

Feel free to contribute to this guide by submitting pull requests or opening issues.

