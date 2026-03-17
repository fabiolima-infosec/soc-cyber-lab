# Phase 3 – Wazuh Installation

This phase focuses on installing and configuring the Wazuh SIEM platform on the Ubuntu Server.

## Objective

Deploy a centralized security monitoring system capable of collecting, analyzing and correlating logs from monitored endpoints.

## Environment

Target machine:

Ubuntu Server  
Role: Wazuh Server  
IP: 192.168.56.10  

## Wazuh Components

The installation includes:

Wazuh Manager  
Wazuh API  
Wazuh Dashboard (Web Interface)  
Filebeat (log forwarding)

## Installation Method

Wazuh was installed using the official installation script.

## Installation Steps

### Step 1 – Update system

sudo apt update && sudo apt upgrade -y

### Step 2 – Download installation script

curl -sO https://packages.wazuh.com/4.7/wazuh-install.sh

### Step 3 – Run installation

sudo bash wazuh-install.sh -a

This installs all Wazuh components in a single-node deployment.

### Accessing the Dashboard

After installation, the Wazuh dashboard is accessible via browser:

https://192.168.56.10

Note:
A security warning may appear due to self-signed certificate.

Default Credentials

Username:
admin

Password:
Generated during installation

### Verification

After installation, the following services were verified:

Wazuh Manager
Wazuh Dashboard
Filebeat

### Status

Wazuh successfully installed and dashboard accessible.
