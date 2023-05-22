---
title: Exercises
description: Exercises in hacking and exploitation
slug: exercises
date: 2023-05-21 00:00:00+0000
toc: true
---

## Bypassing Access Controls

![ ](cameras.jpg)

In this exercise I break a fictitious autograding system to steal other student's assignments and trick it into giving me a good grade. I use my knowledge of file permissions, **setuid Linux programs**, and process isolation to create exploits that take advantage of vulnerabilities I found in the source code. As an exercise in **privilege escalation**, I demonstrate how safelists, input sanitization, and the principle of least privilege can be used to prevent users from circumventing access controls.

**Timeline:** March - April 2023  
**Attacks:** Arbitrary Code Execution, Symlink Traversal, Path Sanitization Bypass  
**Technologies:** Golang, Bash script, Unix

## Hacking a Website

![ ](report.jpg)

I took advantage of a poorly configured website to perform unauthorized actions on its web server. An unsanitaized username field allowed me to create a **SQL injection** attack to bypass a password check on a login page; I used a Stored XSS attack to steal user's cookies that had the HttpOnly flag set to false; By noticing that the website didn't use CSRF tokens, I was able to perform actions on behalf of unsuspecting users who clicked a malicious link to an HTML file with a hidden POST request. My **vulnerability reports** detail the discovery, impact, and mitigation of these and other attacks.

**Timeline:** February - March 2023  
**Attacks:** SQL Injection, Stored XSS, CSRF, Insecure Direct Object Reference  
**Technologies:** HTML, JavaScript, SQL, Burp Suite

## Breaking Weak Cryptography

![ ](crypto.jpg)

Under construction

**Timeline:** February 2023  
**Attacks:** Statistical Cryptanalysis, Meet-in-the-Middle, Brute Force  
**Technologies:** Python, Java

All attacks were performed in a safe and simulated environment.
