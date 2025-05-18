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

## Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

## site:
This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
## Output:
![Screenshot 2025-04-25 092046](https://github.com/user-attachments/assets/3d051aab-768a-4621-9d8a-f0f08b192173)


## filetype: 
This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com
## Output:
![Screenshot 2025-04-25 092305](https://github.com/user-attachments/assets/54bf526a-5363-4117-a84c-8c1907d14d82)

## intext: 
This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
## Output:
![Screenshot 2025-04-25 092636](https://github.com/user-attachments/assets/faf570a2-58af-4f10-ae59-a083dec974ea)

## inurl:
This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
## Output:
![Screenshot 2025-04-25 092820](https://github.com/user-attachments/assets/83e455ef-f3cf-478c-8b74-4ce170aaa1aa)

## intitle: 
This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
## Output:
![Screenshot 2025-04-25 092917](https://github.com/user-attachments/assets/cb4f541f-83e7-4d5d-ae9f-9fa0790984ec)

## link: 
This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
## Output:
![Screenshot 2025-04-25 093039](https://github.com/user-attachments/assets/440a5f24-2565-4a86-b480-6aba72b0c95c)

## cache: 
This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
## Output:
![Screenshot 2025-04-25 093124](https://github.com/user-attachments/assets/6101335f-6a59-4ece-8241-c9ea566fc9c0)

 
# DNS Enumeration
## DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:
![image](https://github.com/user-attachments/assets/61fa8fe6-3939-4df6-a154-db0fa4575d5b)

## dnsenum
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
## Output:
![image](https://github.com/user-attachments/assets/a8474f71-3be2-43a3-b661-301dfcc2c298)

## smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
![image](https://github.com/user-attachments/assets/cbdb32da-96df-4a88-8f1a-2212ef59d7ea)
In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:
![image](https://github.com/user-attachments/assets/84230c5c-5b03-4653-9e62-7fbc3cbba2da)
select any username in the first column of the above file and check the same
## Output:
![image](https://github.com/user-attachments/assets/c6e73ca7-9bb4-45bb-895c-91b2a4622cc1)

# Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands  
## Output:
 ![image](https://github.com/user-attachments/assets/155dd20d-297f-4444-aeee-ba9f973274b9)

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.
## OUTPUT:
![image](https://github.com/user-attachments/assets/bccd668d-2e9d-47d3-925e-dbcde85569ad)

## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

