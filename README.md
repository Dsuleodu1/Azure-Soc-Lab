![](https://www.baeldung.com/wp-content/uploads/sites/4/2023/04/Password-Cracking.png)

# Azure-Soc-Lab

An Azure Sentinel (SIEM) connected to a live virtual machine acting as a honeypot to lure in real life cyber attackers. We will observe live attacks (RDP Brute Force) from all around the world using a custom PowerShell script to look up attackers Geolocation information and then plot it into Azure Sentinel Map to visualize it!

![](https://github.com/Dsuleodu1/Azure-Soc-Lab/blob/main/Screenshot%202025-06-11%20093403.png)

## Features

- Created with Microsoft Azure Sentinel (SIEM) log analytics.
- Provides Knowledge of KQL, PowerShell scripting, remote desktop protocol and virtual machines.
- No installation necessary just create azure free account ![]().
- Gives you hands on experience dropping firewall rules and creating new users to RDP into.
- Allows you to visualize 24hrs of cyber attacks with precise insights on attackers information.
- Works on Mac, Linux and Windows

### Output

![](https://github.com/Dsuleodu1/Azure-Soc-Lab/blob/main/Screenshot%202025-06-11%20093936.png)

> This is the completed visualization of our Microsft Sentinel Log analysis map after 24 hours of monitoring our system. As you can see this visualization presents various locations around the world where our attackers geoIp were found based on our log analytics. Using our PowerShell script we comprised we were able to automate a task in (KQL) Kusto Query Language allowing us to filter out our log analytics to key in on specifications like; time generated, computer, attackerIp, Ipaddres, city name, country name, latitude, and longitude. 

## Tools
- Azure Sentinel, KQL, Virtual Machines, Remote desktop protocol, PowerShell, Windows Event logs
