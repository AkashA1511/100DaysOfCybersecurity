## Day 13 - Introduction to SSRF

### Introduction to SSRF

Today, I solved the TryHackMe lab on Server-Side Request Forgery (SSRF). This lab focuses on exploiting SSRF vulnerabilities, which allow attackers to access internal server resources.

**TryHackMe Lab: [Intro to SSRF](https://tryhackme.com/r/room/ssrfqi)**

#### Key Topics:
- Understanding SSRF Vulnerabilities
- Types of SSRF
- Deny List and Allow List Approaches
- Open Redirect Exploitation

#### Summary:
I learned about different types of SSRF vulnerabilities and how to find and exploit them. The lab covered:

- **Types of SSRF**:
  - Understanding how SSRF vulnerabilities can be exploited to access internal server resources.
  
- **Deny List**:
  - A Deny List accepts all requests except those specified in a list or matching a particular pattern. This approach can be bypassed by using alternative references such as `127.*.*.*`, `0.0.0.0`, `017700000001`, or subdomains resolving to `127.0.0.1`.

- **Allow List**:
  - An Allow List denies all requests unless they match specific rules. Attackers can circumvent this by creating subdomains that fit the allowed pattern.

- **Open Redirect**:
  - Open Redirects are endpoints that automatically redirect visitors to another address. Attackers can use open redirects to bypass SSRF protection by redirecting internal HTTP requests to a domain they control.

---

### Detailed Notes:

**Deny List:**
A Deny List is used to block access to specific resources. However, attackers can bypass this by using alternative references or subdomains that resolve to the blocked IP.

Examples:
- Localhost bypass: `127.1`, `127.*.*.*`, `2130706433`, `017700000001`
- Cloud environment metadata: Block `169.254.169.254` but attackers can use a subdomain pointing to this IP.

**Allow List:**
An Allow List allows requests only if they match specific rules. Attackers can bypass this by creating subdomains that fit the allowed pattern.

Example:
- If the rule is to allow `https://website.thm/*`, attackers can use `https://website.thm.attackers-domain.thm`.

**Open Redirect:**
An open redirect endpoint automatically redirects visitors to another website. Attackers can exploit this to redirect internal HTTP requests to a domain they control.

Example:
- If only URLs beginning with `https://website.thm/` are allowed, attackers can use `https://website.thm/link?url=https://tryhackme.com` to redirect the request.

---

### Summary:
- Completed TryHackMe lab on Introduction to SSRF
- Learned about different types of SSRF and their exploitation techniques
- Studied Deny List and Allow List approaches and how to bypass them
- Understood how Open Redirects can be used in SSRF attacks
- **Today, I will start the PortSwigger lab on SSRF for further practice and deeper understanding.**
