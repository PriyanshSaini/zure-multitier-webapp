# Azure Multi-Tier Web App Deployment (Apache + MySQL)

This project simulates a real-world multi-tier web application hosted on Azure using the free tier.

## Architecture
- **Frontend**: Ubuntu VM with Apache2 and PHP
- **Backend**: Ubuntu VM with MySQL
- **Networking**: Azure Virtual Network with 2 Subnets (Web + DB)
- **Security**: NSGs to isolate tiers and allow necessary access only

## Setup Steps
1. Create Resource Group and VNet with subnets
2. Create and configure NSGs
3. Create Ubuntu VM for Web Tier and install Apache
4. Create Ubuntu VM for DB Tier and install MySQL
5. Allow MySQL connections from Web VM subnet only
6. Test connectivity from Web VM to DB VM using MySQL client

## Files Included
- index.html – Static test page for Apache
