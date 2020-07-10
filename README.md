# Simple LDAP server simulating AD for integration testing

This is a simple LDAP server that tries to simulate an AD using 
Apache Directory Server.

* Should work for activedirectory.js
* Is based on https://github.com/kwart/ldap-server/ and 
   http://stackoverflow.com/questions/11174835/add-memberof-attribute-to-apacheds 


## Docker

1. Build image `docker build -t ldap-ad-it:1.0 .`

2. Run image using
   `docker run -d -p 10389:10389 --name ldap-ad -v <your volume>:/ldap/ldif ldap-ad-it:1.0 `



