# Day 8 - Browser Web Tools and Bug Bounty

**Date:** 2024-31-07

## Summary
Today, I learned about browser web tools and bug bounty hunting. I solved the TryHackMe lab on walking through an application and explored various techniques for reconnaissance in bug bounty hunting.

## Detailed Notes

### Browser Web Tools
I solved the [Walking an Application](https://tryhackme.com/r/room/walkinganapplication) room on TryHackMe, which covered essential browser web tools for understanding and interacting with web applications.

### Bug Bounty - Reconnaissance
I focused on reconnaissance techniques for bug bounty hunting, including passive and active reconnaissance, subdomain enumeration, and using various tools and techniques.

**Reconnaissance:**
Gathering information about the target.

**Two Types:**
1. **Passive Reconnaissance:** The target doesn't know about our presence.
2. **Active Reconnaissance:** The target knows about our presence.

**Subdomain Enumeration:**
Finding associated subdomains.

**Steps to Find Subdomains:**
1. Gather all information.
2. Online tools:
   - [CRT.SH](https://crt.sh/)
   - [CENSYS](https://censys.io)
   - [CertSpotter](https://sslmate.com/certspotter)
3. Public Data Repositories:
   - [VirusTotal](http://virustotal.com)
   - [ThreatCrowd](https://www.threatcrowd.org)
   - [SecurityTrails](https://securitytrails.com)
4. Use Subdomain Enumeration Tools:
   - **Sublist3r:**
     - `Sublist3r -d example.com`
   - **Amass:**
     - `amass enum -d example.com`
   - **Subfinder:**
     - `subfinder -d example.com`
   - **Assetfinder:**
     - `assetfinder -d example.com`

**Google Dorking:**
Using specific Google queries to find subdomains.
- Example: `site:Paytm.com`

**Brute Force Subdomains:**
Tools:
- Wfuzz
- ffuf
- dnsrecon

## Reflections
Today was highly productive, as I got hands-on experience with browser web tools and deepened my understanding of reconnaissance in bug bounty hunting. I'm looking forward to learning about content discovery and further enhancing my skills.

## Next Steps
- Continue with bug bounty learning.
- Explore content discovery techniques.
- Apply the knowledge gained in practical scenarios.
