# Network Architecture

## 🖥️ Overview

The aim is to simulate a small business network enviornment.

The environment consists of:

- 1 Domain Controller (Windows Server)
- 2–4 Client Machines (Windows 10/11)
- Internal virtual network

-----

## 🧱 Core Components

### Domain Controller (DC)

- Hosts Active Directory Domain Services
- Manages authentication and authorisation
- Runs DNS for domain name resolution

-----

### Client Machines

- Windows machines joined to the domain
- Used to simulate end-user environments
- Used for testing policies and troubleshooting

-----

## 🌍 Network Design

- Network Type: Internal (Virtualised)
- Subnet: 192.168.10.0/24

### IP Allocation:

| Device             | IP Address       |
|--------------------|------------------|
| Domain Controller  | 192.168.10.10    |
| Client 1           | 192.168.10.101   |
| Client 2           | 192.168.10.102   |
| Client 3           | 192.168.10.103   |
| Test Machine       | 192.168.10.150   |

-----

## 🌐 Domain Configuration

- Domain Name: `shaun.local`

-----

## 🔑 Key Design Decisions

- Static IP for Domain Controller (required for AD stability)
- Clients will use DC for DNS
- Isolated lab network (for a safe testing environment)
