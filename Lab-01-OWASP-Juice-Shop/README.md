# Lab 01 - OWASP Juice Shop Security Assessment

## Objective

Build a web application security testing lab and perform initial reconnaissance and vulnerability assessment against OWASP Juice Shop.

## Environment

### Attacker Machine

* Parrot OS

### Target Machine

* Ubuntu Server 20.04
* Docker
* OWASP Juice Shop

## Tools Used

* Nmap
* Nikto
* Docker
* Ubuntu Server
* Parrot OS

## Activities Performed

* Deployed OWASP Juice Shop using Docker
* Performed service enumeration using Nmap
* Conducted initial web application assessment using Nikto
* Collected evidence and screenshots

## Status

Lab setup completed successfully.

## Additional Activities Performed

* Configured Burp Suite Community Edition for web traffic interception.
* Intercepted HTTP GET and POST requests from OWASP Juice Shop.
* Captured and analyzed the authentication request endpoint `/rest/user/login`.
* Observed JSON-based credential transmission containing email and password parameters.
* Performed initial authentication flow analysis and request inspection.

## Burp Repeater Activities

* Replayed valid authentication requests using Burp Repeater.
* Performed invalid password testing and analyzed authentication responses.
* Conducted basic parameter manipulation testing on authentication requests.
* Observed token-based authentication responses and server-side validation behavior.
* Compared application responses for valid and invalid authentication attempts.

## JWT Authentication Analysis

* Identified JWT-based authentication mechanism used by OWASP Juice Shop.
* Captured and decoded authentication token using JWT.io.
* Analyzed JWT payload claims including user ID, email, role, and account status.
* Observed token-based session handling and authentication metadata exposure.
