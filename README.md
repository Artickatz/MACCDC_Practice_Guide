# MACCDC_Practice_Guide

## Overview 

"The MACCDC is one of the 9 regional CCDC events in the United States. Now in its 18th year,
our region represents four-year universities and community colleges from Delaware, the
District of Columbia, Maryland, New Jersey, North Carolina, Pennsylvania, Virginia, and West
Virginia. Since its inception, over 3,500 students have participated in the MACCDC.
The MACCDC is one of the 9 regional CCDC events in the United States. Now in its 18th year,
our region represents four-year universities and community colleges from Delaware, the
District of Columbia, Maryland, New Jersey, North Carolina, Pennsylvania, Virginia, and West
Virginia. Since its inception, over 3,500 students have participated in the MACCDC.
This competition consists of both a qualifying round and a regional final round. The virtual
qualifying round took place on February 4th, and the top 8 teams from 26 participating
universities advanced to the in-person regional competition at Prince George’s Community
College on March 31st - April 1st. The winner of the regional competition will advance to the
national round.

The competition is designed to test each student team’s ability to secure networked systems
while maintaining standard business functionality. Each year’s scenario involves team members
simulating a group of employees from a fictitious company who must “inherit-and-defend” an
IT infrastructure. The teams are expected to manage the systems, keep them operational, and
prevent unauthorized access. Each team starts the competition with a set of identically
configured systems. This is not just a technical competition, but also one built upon the
foundation of business operations, policies, and procedures. A technical success that adversely
impacts the business operation will result in a lower score as will a business success which
results in security weaknesses.

Student teams are scored on their ability to detect and respond to outside threats, while
maintaining availability of existing network and application services, responding to business
requests, also known as injects, and balancing security against varying business needs. For more
details, see the Scoring section below." -2023 MACCDC Team Packet

Basically the goal is to have fun and learn while defending systems from real life simulated hackers. 

## Scoring

"Scoring is based on keeping required services up, controlling/preventing unauthorized access,
and completing business tasks (injects) that will be provided throughout the competition." -2023 MACCDDC Team Packet

Every year the vaulue of the scoring and scoring criteria changes though. So be prepeared for that. 

## Rules 

Rules can be found at https://nationalccdc.org/index.php/competition/competitors/rules 

## Enviorment Overview 

Each team usually gets 8 Jump boxes. With 4 being Windows and 4 being Linux based or other. These boxes are usually out of scope and are used to access the cloud based competition infastucture. 

**Example competition enviorment from MACCDC 2023 Regionals team packet**


![image](https://github.com/Artickatz/MACCDC_Practice_Guide/assets/69086568/7ea2cd2f-57d4-44b4-800a-0aed55f6cfa8)


![image](https://github.com/Artickatz/MACCDC_Practice_Guide/assets/69086568/bb00937c-79fb-488c-8ffe-71fe0d77eadd)


| Network Segment | Hostname    | IP Address     | Operating System           |
|------------------|-------------|----------------|----------------------------|
| cloud            | dropbox     | 10.250.20X.13  | Ubuntu 18.04               |
| cloud            | blog        | 10.250.20X.39  | Red Hat 8                  |
| cloud            | intern      | 10.250.20X.42  | Rocky 8                    |
| cloud            | people      | 10.250.20X.55  | Debian 10                  |
| cloud            | customer    | 10.250.20X.88  | Ubuntu 20                  |
| cloud            | office      | 10.250.20X.114 | Ubuntu 20                  |
| cloud            | draw        | 10.250.20X.142 | Rocky 8                    |
| cloud            | inventory   | 10.250.20X.152 | openSUSE 15                |
| cloud            | sso         | 10.250.20X.168 | Windows Server 2016        |
| cloud            | packages    | 10.250.20X.182 | Debian 10                  |
| cloud            | code        | 10.250.20X.194 | Ubuntu 18.04               |
| cloud            | collab      | 10.250.20X.211 | Amazon Linux 2             |
| cloud            | hr          | 10.250.20X.234 | Windows Server 2012 R2     |
| core             | corefw      | 10.250.X.254   | Cisco ASA                  |
| core             | siem        | 10.250.X.19    | Fedora 34                  |
| core             | cdc01       | 10.250.X.20    | Windows Server 2016 Core   |
| core             | automate    | 10.250.X.37    | Amazon Linux 2             |
| core             | edr         | 10.250.X.61    | Amazon Linux 2             |
| core             | coredb      | 10.250.X.100   | Windows Server 2019        |
| core             | connect     | 10.250.X.129   | Palo Alto PAN OS           |
| core             | backups     | 10.250.X.140   | Windows Server 2012 R2     |
| core             | leeroy      | 10.250.X.162   | FreeBSD 12                 |
| core             | keys        | 10.250.X.176   | Windows Server 2016        |
| core             | assets      | 10.250.X.230   | CentOS 7                   |
| hq               | virtual     | 172.2X.0.1     | Proxmox                    |
| hq               | wk1         | 172.2X.0.2     | Gallium OS                 |
| hq               | wk2         | 172.2X.0.3     | Gallium OS                 |
| hq               | wk3         | 172.2X.0.4     | Gallium OS                 |
| hq               | wk4         | 172.2X.0.5     | Gallium OS                 |
| hq               | wk5         | 172.2X.0.6     | Gallium OS                 |
| hq               | wk6         | 172.2X.0.7     | Gallium OS                 |
| hq               | wk7         | 172.2X.0.8     | Windows 10                 |
| hq               | wk8         | 172.2X.0.9     | Windows 10                 |
| hq               | hqdc01      | 172.2X.0.10    | (virtual) Windows Server 2016 |
| hq               | cert        | 172.2X.0.44    | (virtual) Windows Server 2019 |
| hq               | storage     | 172.2X.0.93    | (virtual) Windows Server 2012 R2 |
| hq               | chat        | 172.2X.0.117   | (virtual) Ubuntu 20         |
| hq               | password    | 172.2X.0.139   | (virtual) Rocky 8           |
| hq               | git         | 172.2X.0.173   | (virtual) Rocky 8           |
| hq               | legacy      | 172.2X.0.202   | (virtual) Windows XP        |
| hq               | container   | 172.2X.0.227   | (virtual) Alpine            |
| hq               | fun         | 172.2X.0.234   | (virtual) Alpine            |
| hq               | ap          | 172.2X.0.250   | Dlink DAP-1360C1            |
| hq               | camera      | 172.2X.0.251   | VStarcam C7824WIP           |
| hq               | call        | 172.2X.0.252   | Cisco 7900 VOIP             |
| hq               | hqfw        | 172.2X.0.254   | (virtual) Cisco Firepower   |


## SSH

SSH - Secure Shell
A connection to the server will be made with a specified user, and commands will be executed
as that user. The output of the commands and the ability to connect will be scored.

## HTTP 

HTTP - Hypertext Transfer Protocol
A request for a specific web page will be made and the response will be compared to the
expected result. The returned page must match the expected content for points to be awarded.

## HTTPS

HTTPS - Hypertext Transfer Protocol Secure
A request for a specific web page will be made over SSL. Similarly to HTTP, the response will
compared to the expected value.

## DNS 

DNS - Domain Name System
DNS lookups will be performed against the team’s DNS server. Each successfully served request
will be awarded points.

## LDAP 

LDAP - Lightweight Directory Access Protocol
An authenticated query to the Active Directory LDAP service will be performed.

## FTP 

FTP - File Transfer Protocol
A connection to the server will be made with a specified user, a file will be retrieved, and its
contents will be checked against an expected value.

## SMB 

SMB - Server Message Block
A specified user will attempt to connect to and read a designated file from the remote host.
This file will then be hashed and compared against the expected value.

## WinRM

WinRM - Windows Remote Management
A WinRM session will be created with specified credentials and a command will be executed.

## NFS 

NFS - Network File System
The scoring script will connect to the NFS service and attempt to write to a file. It will then
attempt to log in again and see if the file exists.

## MySQL

MySQL (Database)
A connection to the database will be made with a specified user and a query will be run. The
output of the query will be compared to the expected stored value.

## RDP 

RDP - Remote Desktop
A specified user will attempt to log in via RDP to the service. If a desktop appears, the check will
be successful

## PostgreSQL

PostgreSQL (Database)
Similar to the MySQL check, a connection to the database will be made with a specified user
and a query will be run.

## Elasticsearch 

Elasticsearch
A record will be inserted using the Elasticsearch HTTP API and a request will be made to verify
that the newly created record exists.
