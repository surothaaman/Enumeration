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

![Screenshot 2024-09-18 093807](https://github.com/user-attachments/assets/60d3e176-6100-4016-812b-d61ba6fd65b4)


filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

![Screenshot 2024-09-18 093857](https://github.com/user-attachments/assets/e6acfd44-053d-4e88-8779-91611b8d658f)


intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

![Screenshot 2024-09-18 094013](https://github.com/user-attachments/assets/1a00da45-418c-46a4-88a9-3c4fda88e8ee)


inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

![Screenshot 2024-09-18 094054](https://github.com/user-attachments/assets/ee1273e6-5015-4b7a-8989-e3e0097bb900)

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

![Screenshot 2024-09-18 094841](https://github.com/user-attachments/assets/90b7097f-70e5-4c1b-9d7d-898e572e4fab)

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

![Screenshot 2024-09-18 094939](https://github.com/user-attachments/assets/a30096a4-d669-4f23-bbe8-e502a02f8706)

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

![Screenshot 2024-09-18 095038](https://github.com/user-attachments/assets/acfba47c-a48b-4202-9613-189aeb9d2d57)

 
## DNS Enumeration


## DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:

![Screenshot 2024-09-18 110121](https://github.com/user-attachments/assets/b57ec8db-278c-4752-ab5d-e78fa7b10fcc)




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

![Screenshot 2024-09-18 110613](https://github.com/user-attachments/assets/d8dee227-3eb6-42d4-a5c4-536a32a3d463)

![Screenshot 2024-09-18 110643](https://github.com/user-attachments/assets/36cead05-cb08-4852-9a66-daae87ee3fed)


## smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same


#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ## Output

  ![Screenshot 2024-09-18 110950](https://github.com/user-attachments/assets/c6991bee-51b1-472a-9809-708d2ff63661)

  

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:

![Screenshot 2024-09-18 111112](https://github.com/user-attachments/assets/04455747-8a03-402e-8de1-8282be14af3a)


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

