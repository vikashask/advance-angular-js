### Angular recommends following as security best practices for making sure that your angular app remains secure from some of the most common and known security risks / threats.

1. Ensure to check that requests originate from your web application only, and, not a different website
    Cross-site Request Forgery 

2. Sanitize/Inspect/Validate Users’ Submitted Data

    DomSanitizer and use methods such as following to instruct Angular to not escape the data values because you know that the data values are safe.

    bypassSecurityTrustHtml
    bypassSecurityTrustScript
    bypassSecurityTrustStyle
    bypassSecurityTrustUrl
    bypassSecurityTrustResourceUrl

3. Inspect/Validate Users’ Submitted Data on Server-side code
    Validate all data on server-side code and escape appropriately to prevent XSS vulnerabilities on the server. Angular recommends not to generate Angular templates on the server side using a templating language.

4. Use Offline Template Compiler
    Angular recommends to use offline template compiler to prevent security vulnerabilities called template injection.

5. Implement Content Security Policies (CSP)
    Implement content security policies to avoid attacks such as XSS, Code injection, clickjacking etc

6. Avoid Direct Usage of DOM’s APIs


