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

Vulnerability #1:__SQL Injection__  
 * Blind SQL injection can be run by inserting ' OR SLEEP(5)=0--' at the end of the URL within the salesperson page. For example: https://35.226.11.110/blue/public/salesperson.php?id=%27%20OR%20SLEEP(5)=0--%27 makes the page load for 5 seconds.

Vulnerability #2: __________________


## Green

Vulnerability #1: __Username Enumeration__
 * If an existing username is entered with the incorrect password, the failure message appears in bold. If a username that does not exist is used, the error message is in non-bold text. Upon checking the source code, this is because these errors were stored as different classes, one called "failed" and one called "failure".
 ![alt text](https://github.com/etseff/Seff_CPWeek8/blob/master/InkedScreenshot%202018-04-04%2019.07.26_LI.jpg)

Vulnerability #2: __Cross-Site Scripting__
 * The Contact page has a cross-site scripting vulnerability. Script like <script>alert('Elie found the XSS!');</script> can be added in the contact form, then upon logging in as admin and clicking the feedback tab, the alert popped up.

## Red

Vulnerability #1: __Insecure Direct Object Reference__
 * On the red pag under the "Find a Salesperson" tab, clicking through the salespeople reveals the vulnerability because at the end of each URL is salesperson.php?id=N, where N is a number. By using https://35.226.11.110/red/public/salesperson.php?id=10, I was able to find a salesperson whose page is not supposed to be public. 

Vulnerability #2: __________________


## Notes

Describe any challenges encountered while doing the work
