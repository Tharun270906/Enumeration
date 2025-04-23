##DEVELOPED BY:
```
A.Tharun
212224100060
```
# Enumeration
Enumeration Techniques

# Explore Google hacking and enumeration 

# AIM:

To use Google for gathering information and perform enumeration of targets

## STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various Google hacking keywords and enumeration tools as follows:


### Step 3:
Open terminal and try execute some kali linux commands

## Pen Test Tools Categories:  

Following Categories of pen test tools are identified:
Information Gathering.

Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com
![image](https://github.com/user-attachments/assets/0b5fdbaa-18d7-429b-a958-9e4b70ebf27f)

filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com
![image](https://github.com/user-attachments/assets/0d0715a8-2efb-438f-8d68-2648024a3640)


intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
![image](https://github.com/user-attachments/assets/2fc25f53-741d-4c36-ab1f-734e413ff5fb)


inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
![image](https://github.com/user-attachments/assets/617ecaf4-84e8-4762-8011-fc1df0792c76)


intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
![image](https://github.com/user-attachments/assets/e90fc8cf-a6bf-453b-9d3b-f992e18c0331)


link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
![image](https://github.com/user-attachments/assets/bf33fab4-9dc5-484e-b0a3-6bc67c1f90d3)

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
![image](https://github.com/user-attachments/assets/def5f6fe-5d9a-4129-8095-ce6845f44a62)


#DNS Enumeration
##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
![Screenshot 2025-04-23 214153](https://github.com/user-attachments/assets/ca71fbb2-51d1-45a3-9a38-86a7d8af0cd8)
![Screenshot 2025-04-23 214727](https://github.com/user-attachments/assets/e05c0779-fe7e-4511-9e45-f270666097fe)

##dnsenum
Dnsenum is a multithreaded perl script to enumerate DNS information of a domain and to discover non-contiguous ip blocks. The main purpose of Dnsenum is to gather as much information as possible about a domain. The program currently performs the following operations:

Get the host’s addresses (A record).
Get the namservers (threaded).
Get the MX record (threaded).
Perform axfr queries on nameservers and get BIND versions(threaded).
Get extra names and subdomains via google scraping (google query = “allinurl: -www site:domain”).
Brute force subdomains from file, can also perform recursion on subdomain that have NS records (all threaded).
Calculate C class domain network ranges and perform whois queries on them (threaded).
Perform reverse lookups on netranges (C class or/and whois netranges) (threaded).
Write to domain_ips.txt file ip-blocks.
This program is useful for pentesters, ethical hackers and forensics experts. It also can be used for security tests.
## OUTPUT:
![image](https://github.com/user-attachments/assets/e5b0f2e8-9c72-4f29-9cf2-d7d1d199e49f)

##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
![Screenshot 2025-04-23 220834](https://github.com/user-attachments/assets/a1d2203b-3dcc-47e9-aab7-6e2dc616c2ce)

In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:
##Output:
![Screenshot 2025-04-23 221102](https://github.com/user-attachments/assets/a110ed18-b2a9-4d8e-9d07-56ad3e1e3735)

select any username in the first column of the above file and check the same
##Output:
![Screenshot 2025-04-23 221426](https://github.com/user-attachments/assets/50362558-ece1-4e04-95f9-b47001fe6e6c)

#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ##Output
 ![Screenshot 2025-04-23 222723](https://github.com/user-attachments/assets/c2d96179-2f77-49d7-91dc-0e332de86420)
 
## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.

## OUTPUT:
![Screenshot 2025-04-23 223410](https://github.com/user-attachments/assets/711d7d0e-493f-4c96-aae6-a1b74778a8f0)


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

