# Learn-SecByte-CTF-Labs-Collection-Log4Shell-Spring4Shell-ProxyShell-Windows-LPE
A curated collection of hands-on cybersecurity CTF labs covering Log4Shell, Spring4Shell, ProxyLogon/ProxyShell, Microsoft SharePoint, Windows CLFS LPE, and Apache Framework CVEs from Learn SecByte.
# Learn SecByte CTF & Cybersecurity Labs Collection

Welcome to the **Learn SecByte CTF & Cybersecurity Labs Collection**. This repository is a dedicated, searchable index of hands-on Java framework exploits (Log4Shell, Spring4Shell, Apache Struts 2, Apache Solr, Apache OFBiz), web server path traversal RCEs (Apache HTTP Server), enterprise Microsoft suite vulnerabilities (ProxyLogon, ProxyShell, SharePoint, Azure AD Connect), and kernel-level Windows Local Privilege Escalation (CLFS Driver) designed for cybersecurity students, CTF players, vulnerability researchers, security analysts, and enterprise penetration testers.

---

## Table of Contents
- [Introduction](#introduction)
- [Lab Collection & Index](#lab-collection--index)
- [Categories](#categories)
- [Learning Path](#learning-path)
- [How to Use the Labs](#how-to-use-the-labs)
- [Disclaimer](#disclaimer)

---

## Introduction

Enterprise application servers, Java framework stacks, web servers, and Windows core kernel drivers form the primary attack surface targeted by threat actors to achieve initial access, remote code execution, and system takeover. Hosted on [Learn SecByte](https://learn.secbyte.org/), this advanced Java framework, web server, Microsoft enterprise ecosystem, and Windows kernel privilege escalation collection provides practical, hands-on technical training to analyze, reproduce, and mitigate critical software vulnerabilities.

From understanding JNDI lookup injection in Apache Log4j (`Log4Shell`), ClassLoader manipulation in Spring Framework (`Spring4Shell`), Jakarta Multipart parser injection in Apache Struts 2, and path traversal normalized character bypasses in Apache HTTP Server to chaining SSRFs and PowerShell remoting on Microsoft Exchange (`ProxyLogon` & `ProxyShell`), bypassing JWT authentication on SharePoint, and exploiting out-of-bounds array writes in the Windows CLFS kernel driver, these exercises equip practitioners to defend core enterprise infrastructure.

---

## Lab Collection & Index

Below is the complete, searchable index of all Java framework, Apache server, Microsoft enterprise platform, and Windows kernel CVE challenges in this collection:

| # | Lab / Challenge Name | Category | Focus / Key Topics | Lab Link |
|---|----------------------|----------|---------------------|----------|
| 1 | **Log4Shell: Apache Log4j RCE Defense and Exploitation Lab** | Java Ecosystem & Web Framework CVEs | JNDI LDAP lookup injection, remote class loading, unauthenticated remote code execution, Log4j string substitution defense | [Access Lab](https://learn.secbyte.org/ctf/log4shell-apache-log4j-rce-defense-and-exploitation-lab) |
| 2 | **Spring4Shell CVE-2022-22965 Remote Code Execution** | Java Ecosystem & Web Framework CVEs | Spring Framework DataBinder ClassLoader manipulation, Tomcat AccessLogValue modification, web shell placement | [Access Lab](https://learn.secbyte.org/ctf/spring4shell-cve-2022-22965-remote-code-execution) |
| 3 | **Apache Struts 2 CVE-2017-5638 RCE** | Java Ecosystem & Web Framework CVEs | Jakarta Multipart parser exception handling flaw, OGNL expression injection in `Content-Type` headers, remote command execution | [Access Lab](https://learn.secbyte.org/ctf/apache-struts-2-cve-2017-5638-rce) |
| 4 | **Apache Solr CVE-2019-0193 Remote Code Execution** | Java Ecosystem & Web Framework CVEs | DataImportHandler (DIH) module script configuration, custom JavaScript payload injection, unauthenticated remote code execution | [Access Lab](https://learn.secbyte.org/ctf/apache-solr-cve-2019-0193-remote-code-execution) |
| 5 | **Apache OFBiz Authentication Bypass CVE-2023-49070** | Java Ecosystem & Web Framework CVEs | XML-RPC request parser flaw, unauthenticated API endpoint access, deserialization vector trigger, security control bypass | [Access Lab](https://learn.secbyte.org/ctf/apache-ofbiz-authentication-bypass-cve-2023-49070) |
| 6 | **Apache HTTP Server CVE-2021-41773 Path Traversal RCE** | Web Server & Path Traversal CVEs | URL path normalization bypass (`.%2e`), arbitrary file reading, CGI script execution when cgi-bin is enabled | [Access Lab](https://learn.secbyte.org/ctf/apache-http-server-cve-2021-41773-path-traversal-rce) |
| 7 | **Apache CVE-2021-42013 Path Traversal RCE** | Web Server & Path Traversal CVEs | Incomplete fix for CVE-2021-41773, double URL encoding bypass (`%%32%65`), system file disclosure, remote code execution | [Access Lab](https://learn.secbyte.org/ctf/apache-cve-2021-42013-path-traversal-rce) |
| 8 | **ProxyLogon: Microsoft Exchange SSRF Initial Access** | Microsoft Enterprise Suite & Cloud Infrastructure | Pre-authentication Server-Side Request Forgery (CVE-2021-26855), backend impersonation, arbitrary file write via ECP | [Access Lab](https://learn.secbyte.org/ctf/proxylogon-microsoft-exchange-ssrf-initial-access) |
| 9 | **Microsoft Exchange ProxyShell RCE CVE-2021-34473** | Microsoft Enterprise Suite & Cloud Infrastructure | Pre-auth path confusion (CVE-2021-34473), PowerShell backend elevation (CVE-2021-34523), arbitrary file write (CVE-2021-31207) | [Access Lab](https://learn.secbyte.org/ctf/microsoft-exchange-proxyshell-rce-cve-2021-34473) |
| 10 | **Microsoft SharePoint Server CVE-2023-29357 Authentication Bypass** | Microsoft Enterprise Suite & Cloud Infrastructure | OAuth token signature validation flaw, spoofed JWT token processing, site collection administrative impersonation | [Access Lab](https://learn.secbyte.org/ctf/microsoft-sharepoint-server-cve-2023-29357-authentication-by) |
| 11 | **Microsoft Azure AD Connect CVE-2021-36949 Privilege Escalation** | Microsoft Enterprise Suite & Cloud Infrastructure | Password hash extraction from local database storage, administrative account takeover, hybrid cloud domain escalation | [Access Lab](https://learn.secbyte.org/ctf/microsoft-azure-ad-connect-cve-2021-36949-privilege-escalati) |
| 12 | **Windows CLFS Driver LPE CVE-2023-28252** | Windows Kernel & Local Privilege Escalation | Out-of-bounds array write in Common Log File System (`clfs.sys`) driver, kernel memory corruption, SYSTEM privilege escalation | [Access Lab](https://learn.secbyte.org/ctf/windows-clfs-driver-lpe-cve-2023-28252) |

---

## Categories

### 1. Java Ecosystem & Web Framework CVEs
Audit high-severity vulnerabilities across Java enterprise software, including Log4j JNDI injection (`Log4Shell`), Spring Framework DataBinder ClassLoader manipulation (`Spring4Shell`), Apache Struts 2 OGNL injection, Apache Solr DIH scripting, and Apache OFBiz XML-RPC auth bypasses.
- [Log4Shell: Apache Log4j RCE Defense and Exploitation Lab](https://learn.secbyte.org/ctf/log4shell-apache-log4j-rce-defense-and-exploitation-lab)
- [Spring4Shell CVE-2022-22965 Remote Code Execution](https://learn.secbyte.org/ctf/spring4shell-cve-2022-22965-remote-code-execution)
- [Apache Struts 2 CVE-2017-5638 RCE](https://learn.secbyte.org/ctf/apache-struts-2-cve-2017-5638-rce)
- [Apache Solr CVE-2019-0193 Remote Code Execution](https://learn.secbyte.org/ctf/apache-solr-cve-2019-0193-remote-code-execution)
- [Apache OFBiz Authentication Bypass CVE-2023-49070](https://learn.secbyte.org/ctf/apache-ofbiz-authentication-bypass-cve-2023-49070)

### 2. Web Server Path Traversal & Remote Code Execution
Analyze URL normalization flaws in web servers, bypassing path validation in Apache HTTP Server via single and double URL-encoded sequences to read files and execute CGI scripts.
- [Apache HTTP Server CVE-2021-41773 Path Traversal RCE](https://learn.secbyte.org/ctf/apache-http-server-cve-2021-41773-path-traversal-rce)
- [Apache CVE-2021-42013 Path Traversal RCE](https://learn.secbyte.org/ctf/apache-cve-2021-42013-path-traversal-rce)

### 3. Microsoft Enterprise Suite & Cloud Infrastructure
Master exploit chains targeting Microsoft enterprise software, including ProxyLogon SSRFs, ProxyShell path confusion and PowerShell remoting, SharePoint OAuth JWT authentication bypasses, and Azure AD Connect database credential harvesting.
- [ProxyLogon: Microsoft Exchange SSRF Initial Access](https://learn.secbyte.org/ctf/proxylogon-microsoft-exchange-ssrf-initial-access)
- [Microsoft Exchange ProxyShell RCE CVE-2021-34473](https://learn.secbyte.org/ctf/microsoft-exchange-proxyshell-rce-cve-2021-34473)
- [Microsoft SharePoint Server CVE-2023-29357 Authentication Bypass](https://learn.secbyte.org/ctf/microsoft-sharepoint-server-cve-2023-29357-authentication-by)
- [Microsoft Azure AD Connect CVE-2021-36949 Privilege Escalation](https://learn.secbyte.org/ctf/microsoft-azure-ad-connect-cve-2021-36949-privilege-escalati)

### 4. Windows Kernel & Local Privilege Escalation (LPE)
Examine low-level Windows kernel driver memory corruption, triggering out-of-bounds array writes in `clfs.sys` to escalate from standard local user to `NT AUTHORITY\SYSTEM`.
- [Windows CLFS Driver LPE CVE-2023-28252](https://learn.secbyte.org/ctf/windows-clfs-driver-lpe-cve-2023-28252)

---

## Learning Path

Follow this structured progression path to master web server path traversal, Java framework exploit development, Microsoft enterprise platform compromise, and Windows kernel privilege escalation:

1. **Phase 1: Web Server Path Traversal & Java Framework Exploitation** — Dissect URL encoding bugs and master Java injection vectors (`Log4Shell`, `Spring4Shell`, Struts 2):
   - [Apache HTTP Server CVE-2021-41773 Path Traversal RCE](https://learn.secbyte.org/ctf/apache-http-server-cve-2021-41773-path-traversal-rce)
   - [Apache CVE-2021-42013 Path Traversal RCE](https://learn.secbyte.org/ctf/apache-cve-2021-42013-path-traversal-rce)
   - [Apache Struts 2 CVE-2017-5638 RCE](https://learn.secbyte.org/ctf/apache-struts-2-cve-2017-5638-rce)
   - [Log4Shell: Apache Log4j RCE Defense and Exploitation Lab](https://learn.secbyte.org/ctf/log4shell-apache-log4j-rce-defense-and-exploitation-lab)
   - [Spring4Shell CVE-2022-22965 Remote Code Execution](https://learn.secbyte.org/ctf/spring4shell-cve-2022-22965-remote-code-execution)

2. **Phase 2: Database & Management Framework Flaws** — Research unauthenticated API access and custom script injections in Solr and OFBiz:
   - [Apache Solr CVE-2019-0193 Remote Code Execution](https://learn.secbyte.org/ctf/apache-solr-cve-2019-0193-remote-code-execution)
   - [Apache OFBiz Authentication Bypass CVE-2023-49070](https://learn.secbyte.org/ctf/apache-ofbiz-authentication-bypass-cve-2023-49070)

3. **Phase 3: Microsoft Enterprise Ecosystem & Mail Gateway Compromise** — Chain SSRFs, JWT bypasses, and PowerShell remoting across Exchange, SharePoint, and Azure AD Connect:
   - [Microsoft Azure AD Connect CVE-2021-36949 Privilege Escalation](https://learn.secbyte.org/ctf/microsoft-azure-ad-connect-cve-2021-36949-privilege-escalati)
   - [Microsoft SharePoint Server CVE-2023-29357 Authentication Bypass](https://learn.secbyte.org/ctf/microsoft-sharepoint-server-cve-2023-29357-authentication-by)
   - [ProxyLogon: Microsoft Exchange SSRF Initial Access](https://learn.secbyte.org/ctf/proxylogon-microsoft-exchange-ssrf-initial-access)
   - [Microsoft Exchange ProxyShell RCE CVE-2021-34473](https://learn.secbyte.org/ctf/microsoft-exchange-proxyshell-rce-cve-2021-34473)

4. **Phase 4: Windows Kernel Subsystems & Local Privilege Escalation** — Analyze kernel-mode driver memory corruption and trigger local SYSTEM privilege escalation:
   - [Windows CLFS Driver LPE CVE-2023-28252](https://learn.secbyte.org/ctf/windows-clfs-driver-lpe-cve-2023-28252)

---

## How to Use the Labs

1. Select a challenge link from the index or category sections above.
2. Read the scenario directives, software version specifications, and vulnerability details on [Learn SecByte](https://learn.secbyte.org/).
3. Deploy analysis toolsets (Burp Suite, Python, Marshalsec, Rogue-JNDI, Metasploit, PowerShell, WinDbg) inside an isolated workstation or virtual machine.
4. Craft JNDI lookup payloads, forge JWT tokens, execute Exchange PowerShell commands, trigger CLFS kernel memory corruptions, and capture target flags.

---

## Disclaimer

This repository and its linked challenge resources are strictly intended for educational, threat research, and authorized technical security training purposes. Never attempt to execute Log4Shell payloads, ProxyShell exploit chains, JWT forge attempts, or kernel driver memory corruption exploits against unauthorized production networks, public cloud environments, or third-party enterprise infrastructure.
