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
- Scan a single host: `nmap 192.168.1.1`
- Scan a range of IP addresses: `nmap 192.168.1.1-100`
- Scan a specific port: `nmap -p 80 192.168.1.1`
- Perform an aggressive scan: `nmap -A 192.168.1.1`

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

