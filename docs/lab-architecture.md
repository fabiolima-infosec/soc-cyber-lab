# SOC Cybersecurity Home Lab

## Objective

Build a Security Operations Center (SOC) laboratory to simulate cyber attacks and analyze them using Wazuh.

## Infrastructure

The environment is built using Oracle VirtualBox.

Virtual machines:

Kali Linux
Role: Attacker machine

Ubuntu Server
Role: Wazuh Server (SOC monitoring)

Windows Server 2022
Role: Monitored endpoint

## Network

VirtualBox Host-Only Network

Internal network range:
192.168.56.0/24

Example IPs:

Ubuntu Wazuh Server
192.168.56.10

Kali Linux
192.168.56.20

Windows Server
192.168.56.30
