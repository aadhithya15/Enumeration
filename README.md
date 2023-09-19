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

### site: 
This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com
## Output:
![239720288-29828d11-353b-40d3-8951-61a42d9c029f](https://github.com/Yogeshvar005/Enumeration/assets/113497367/b0d2e5dc-45c3-4e7d-b2b6-489f7f4d4abf)


### filetype: 
This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com
## Output:
![239720300-f169a7de-0f7f-4b8c-b402-ccaa6ea6a907](https://github.com/Yogeshvar005/Enumeration/assets/113497367/50763ff5-d7f9-4dc7-b2bc-7367d4e00753)





### intext: 
This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
## Output:
![239720307-f7716744-5455-463e-b0a0-3a44821e70af](https://github.com/Yogeshvar005/Enumeration/assets/113497367/5cb92ff7-1ed6-4a43-804d-77e9cb30e8b9)



### inurl: 
This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
## Ouput:
![239720312-61b83322-2aba-44f3-9a90-dc9bb3fe6175](https://github.com/Yogeshvar005/Enumeration/assets/113497367/0d32a079-4241-4ff9-b748-f020ecbaadd9)


### intitle: 
This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
## Output:
![239720322-cbda231f-5058-4343-8541-014cc1c5729c](https://github.com/Yogeshvar005/Enumeration/assets/113497367/83f8a230-9ece-4484-b062-dea17af8261e)


### link: 
This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
## Output:
![239720329-bf1840b8-075d-497e-8f1c-4ca6d8327982](https://github.com/Yogeshvar005/Enumeration/assets/113497367/c17f94f1-60b1-4083-b842-4a272005190e)


### cache: 
This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
## Output:
![239720337-e127c95b-a133-42d4-aa3d-a833faa3aad0](https://github.com/Yogeshvar005/Enumeration/assets/113497367/8e479e7c-f00f-42bb-a3e6-5b13058325c9)

 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:

![241196881-e27b6257-4d38-4365-a04f-6bd71610632a](https://github.com/Yogeshvar005/Enumeration/assets/113497367/883538b0-a495-48f9-aa52-38d0fb67e3e5)






##Dnsenum
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

![241198023-795c489d-ba57-4e77-9791-49c71fc3f4d3](https://github.com/Yogeshvar005/Enumeration/assets/113497367/2c0be4b0-705e-4c3f-9658-bb773e95a5b0)

##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
![241410635-c41be6f0-d0d4-40eb-9074-136cabe5c74b](https://github.com/Yogeshvar005/Enumeration/assets/113497367/861d02e6-ad2e-4f7f-b9b5-2521cb6d7b1d)


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:
![241408341-ba786664-2105-44aa-ab07-465057083629](https://github.com/Yogeshvar005/Enumeration/assets/113497367/b740c9e8-14ca-49c8-8c5b-87e703fe36cb)

select any username in the first column of the above file and check the same

![241408615-ad0d26fe-7a60-4604-be93-1bf950d88646](https://github.com/Yogeshvar005/Enumeration/assets/113497367/e0bd992a-a093-4521-9190-e377286c4a74)

#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ##Output
  
  ![241409971-4fd9ca59-abdf-43bc-917c-71e2c7e4351d](https://github.com/Yogeshvar005/Enumeration/assets/113497367/a8470755-3ba8-48a1-b5fc-453a250d2fe6)


## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:

![241410190-9ca27cef-c123-4ab2-b4b1-13e67d6e6d19](https://github.com/Yogeshvar005/Enumeration/assets/113497367/9bd4c245-dd84-4517-bf27-12a7cd3c070b)

## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully
