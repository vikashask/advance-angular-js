### Angular recommends following as security best practices for making sure that your angular app remains secure from some of the most common and known security risks / threats.

### Ensure to check that requests originate from your web application only, and, not a different website
    Cross-site Request Forgery 

### Sanitize/Inspect/Validate Users’ Submitted Data

    DomSanitizer and use methods such as following to instruct Angular to not escape the data values because you know that the data values are safe.

    bypassSecurityTrustHtml
    bypassSecurityTrustScript
    bypassSecurityTrustStyle
    bypassSecurityTrustUrl
    bypassSecurityTrustResourceUrl

### Inspect/Validate Users’ Submitted Data on Server-side code
    Validate all data on server-side code and escape appropriately to prevent XSS vulnerabilities on the server. Angular recommends not to generate Angular templates on the server side using a templating language.

### Use Offline Template Compiler
    Angular recommends to use offline template compiler to prevent security vulnerabilities called template injection.

### Implement Content Security Policies (CSP)
    Implement content security policies to avoid attacks such as XSS, Code injection, clickjacking etc

### Avoid Direct Usage of DOM’s APIs
    Angular recommends using Angular template rather than using DOM’s APIs such as Document, ElementRef etc. directly.

### Prefix JSON Responses to Make Them Non-Executable
    This is related with security vulnerability/issue, Cross-Site Script Inclusion (XSSI). The security risk/vulnerability exploits aspect of executing JSON response as Javascript.

### Up-to-date Angular Libraries

### Avoid Modifying the Angular Copy
    This is to make sure that it does not create hard links in between your application and angular versions so much so that you become unable to upgrade to newer Angular versions.

### Audit & Test Everything at Regular Intervals



