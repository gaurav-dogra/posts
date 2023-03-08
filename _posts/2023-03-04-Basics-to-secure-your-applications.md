---
layout: post
category: App Security
---
## App Security for Developers

App Security is critical consideration for developers, as it helps to ensure that the applications they create are safe, 
reliable, and trustworthy for users. 

I am doing Application Security Training from immersivelabs.online. And I have made the following notes

App security for developers typically involves the following key aspects:

1. Insecure deserialization 
    * Serialization is converting an object/data to XML/JSON so that it can be stored or transmitted.
    * Deserialization is reverse of Serialization
    * Insecure deserialization vulnerabilities occur when untrusted user input is parsed in insecure manner
    * An attacker can send an XML/JSON object which can alter the unintended properties, or worse, introduce additional code which would be executed by the language or framework the application is running in
    * So developer should be use libraries that are known to perform deserialization securly
2. Use Strong Authentication measures
   * Authentication is the process of verifying the identity of a user, typically through the use of a username and password, OTP, or other factors such as biometric authentication. 
   * Authentication can also be used to enforce accountability, by keeping a record of who has accessed the system and when. This can help to deter insider threats and to identify and respond to security incidents.
3. Proper Authorization
   * Authorization is the process of granting or denying access to specific resources or actions based on a user's identity, role, or other factors.
   * This helps to prevent unauthorized access, data breaches, and other security risks.
   * For example, in a web application, authorization can be used to control access to specific pages or functions based on a user's login credentials or role. 
4. The principle of least privilege 
   * It is a security principle that states that users or entities should be granted only the minimum level of access or permissions necessary to perform their required tasks, and no more.
5. Security Patching 
   * Applying patches in a timely manner removes the risks associated with known vulnerabilities.
6. Secure Session Management
   * Session fixation: where an attacker sets the session ID of a victim before they authenticate, allowing the attacker to hijack the session once the user logs in.
   * Session prediction: where an attacker can predict or guess the session ID of a user's session, allowing them to hijack the session.
   * Session hijacking: where an attacker intercepts a user's session ID or other session information and uses it to impersonate the user.
   * To prevent broken session management vulnerabilities, applications should implement 
     * generating strong and unpredictable session IDs
     * enforcing session timeouts
     * invalidating sessions after logout
     * regularly test and audit session management mechanisms
7. Code Comments
     * Developers often leave comments in their code to help other developers or themselves upon returning.
     * Sensitive details may be included in code comments include passwords, access tokens, API keys, database credentials, and other authentication or authorization information. 
8. Default Error Pages
     * Applications that return default error pages may leak sensitive information, such as the server software and version in use
     * Use Custom Error pages
9. Log the below
     * Log Successful Login and unsuccessful logins
     * logouts
     * Password changes and reset attempts
     * Creation, removal, and changes to user's authorisation
     * Authorisation failures
     * Who has Accessed the sensitive data
     * Input validation failures
   
    

       
