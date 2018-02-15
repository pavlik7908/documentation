# RUPAYA Hot + Cold wallet MasterNode setup guide

> This is a community contributed guide. Feel free to suggest improvements via Issues or opening Pull Requests. Thank you!

**!!! This guide is for setting up a new MasterNode using the new (dark theme) Rupaya v4 wallet and chain !!!**

## Setup overview


### Hot Wallet
In this guide, we refer to **Hot** wallet as the Rypaya wallet (Linux or Windows) that is running on the MasterNode server, with public IP address on it, providing services to the blockchain network for which it's rewarded with coins.
It's **Hot** because it's out on the public internet 24/7, directly accessible on the peer-to-peer port (TCP 9020), much more vulnerable than a cold. Fortunatelly this wallet is running with a balance of 0 coins.
It's strongly recommended not to run MasterNode Hot wallet at home! See a list of reasons here: TODO 

### Cold Wallet
We refer to **Cold** wallet as the Rypaya wallet (Windows, OSX, Linux) that holds the RUPX collateral and is used to enable the MasterNode(s) and collect rewards for services.
This is normally run at home, behind firewall, without direct connectivity from the internet, making it a more secure 

---

## Requirements

### Hot Wallet
* Ubuntu 14.04 or 16.04 running on a VPS such as Vultr, or other server (This will be your Hot wallet) running 24/7
* Static IP Address
* Port 5500 port forwarded from your router to your Ubuntu server
* Basic Linux skills

### Cold Wallet
* Windows 7 or higher (This will be your Cold wallet)

---