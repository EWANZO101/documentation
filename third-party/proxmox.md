---
title: Proxmox
description: This guide explains how you can setup the proxmox integration with WemX
published: true
date: 2023-12-03T17:08:54.232Z
tags: 
editor: markdown
dateCreated: 2023-12-03T17:08:09.490Z
---

# Installing the Proxmox Service

1. Download the latest Proxmox Service ZIP: https://github.com/WemXPro/service-proxmox/archive/refs/heads/main.zip
2. Using FTP, locate folder /var/www/wemx/app/Services and create a new folder called Proxmox
3. Open the ZIP file downloaded earlier, then open service-proxmox-main folder
4. Upload all files in this folder to the Proxmox folder in /var/www/wemx/app/Services/Proxmox
5. Update the Proxmox dependencies with php artisan module:update Proxmox

# Setup Proxmox service

After installing Proxmox, head over to Admin -> Services -> Enable Proxmox

![hestia-services.png](/assets/hestia-services.png)

After enabling Proxmox, click on Configuration

![proxmox-config.png](/assets/proxmox-config.png)

- Hostname: Enter the URL to your Proxmox panel including http:// or https:// and port
![step_1_login_.png](/assets/step_1_login_.png)
You can create a new token on your Proxmox panel under Datacenter -> API Tokens -> Add
![part_5.png](/assets/part_5.png)

![part_6.png](/assets/part_6.png)
You can create a new token,u can use a random password generater like this one www.random.org/passwords/?num=1&len=24&format=plain&rnd=new 
![SVAE_7.png](/assets/SVAE_7.png)

![TOKEN_6.png](/assets/TOKEN_6.png)
copy the token id and password once it has been generated.

Then head over to your store and go to 
/admin/services
![steup_store.png](/assets/steup_store.png)

![store_2.png](/assets/store_2.png)

Test connection u should see - Successfully connected with Proxmox 



