# Phase 1 – Virtual Machine Setup

This phase focuses on building the infrastructure of the SOC laboratory.

## Virtualization Platform

Oracle VirtualBox  
Version: Versão 7.2.6 r172322

## Network Architecture

Network type: Host-Only Adapter

Network range:
192.168.56.0/24

Purpose:
Allow communication between lab machines while keeping the environment isolated from the host network.

## Virtual Machines

Three virtual machines were created.

### Kali Linux

Purpose:
Attack simulation

Operating System:
Kali Linux (version)

Resources:
CPU: 1 core  
RAM: 4 GB  
Disk: 25 GB (VDI)

Network:
Host-Only Adapter

IP Address:
192.168.56.20

---

### Ubuntu Server

Purpose:
Host the Wazuh server

Operating System:
Ubuntu Server (version)

Resources:
CPU: 1 core  
RAM: 6 GB  
Disk: 25 GB (VDI)

Network:
Host-Only Adapter

IP Address:
192.168.56.10

---

### Windows Server 2022

Purpose:
Monitored endpoint for Wazuh agent

Operating System:
Windows Server 2022

Resources:
CPU: 1 core  
RAM: 4 GB  
Disk: 50 GB (VDI)

Network:
Host-Only Adapter

IP Address:
192.168.56.30

---

## Status

All machines are able to communicate with each other using ICMP (ping).
