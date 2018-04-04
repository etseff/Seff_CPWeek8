# Seff_CPWeek8
CodePath Week 8 Assignment
# Project 8 - Pentesting Live Targets

Time spent: **X** hours spent in total

> Objective: Identify vulnerabilities in three different versions of the Globitek website: blue, green, and red.

The six possible exploits are:
* Username Enumeration
* Insecure Direct Object Reference (IDOR)
* SQL Injection (SQLi)
* Cross-Site Scripting (XSS)
* Cross-Site Request Forgery (CSRF)
* Session Hijacking/Fixation

Each version of the site has been given two of the six vulnerabilities. (In other words, all six of the exploits should be assignable to one of the sites.)

## Blue

Vulnerability #1:________________  

Vulnerability #2: __________________


## Green

Vulnerability #1: __Username Enumeration__
 * If an existing username is entered with the incorrect password, the failure message appears in bold. If a username that does not exist is used, the error message is in non-bold text. Upon checking the source code, this is because these errors were stored as different classes, one called "failed" and one called "failure".

Vulnerability #2: __________________


## Red

Vulnerability #1: __Insecure Direct Object Reference__
 * On the red pag under the "Find a Salesperson" tab, clicking through the salespeople reveals the vulnerability because at the end of each URL is salesperson.php?id=N, where N is a number. By using https://35.226.11.110/red/public/salesperson.php?id=10, I was able to find a salesperson whose page is not supposed to be public. 

Vulnerability #2: __________________


## Notes

Describe any challenges encountered while doing the work
