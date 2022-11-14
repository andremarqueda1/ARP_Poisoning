# ARP Poisoning and MiTM Attack
The objective of this project is to sniff a certain device traffic. 

**"Sniffing"** is the action of **intercepting another device's traffic (without the other user's acknowledgment) and capturing it for further analysis.** For this, I'll be using the technique known as ***ARP Poisoning*** (more info below). 

I'll use my home network for this example.  

## Step 0 | What do I need?
There are a variety of free tools available for Windows, Mac and Linux. For simplicity, in this example we will be using a Linux distribution with a variety of pen-testing software included, (but you can use any Linux distribution): 

 - Kali Linux 2022.3 
 - nMap 7.80
 - Ettercap 0.8.3

To install the required software, run:

    sudo apt get install nmap
    sudo apt get install ettercap-text-only
*We do not need the GUI for Ettercap*



## Step 1 | Where Am I?
First we have to do some reconnaissance. We'll need the gateway IP:  
> ip r | grep default
[](https://raw.githubusercontent.com/andremarqueda1/ARP_Poisoning/main/images/1%20-%20gateway.jpg)
