## HTTPS & SSL
- HTTPS (Hypertext Transfer Protocol Secure) relies on SSL (Secure Sockets Layer) or its successor TLS (Transport Layer Security) to secure communication over a network. The main roles of SSL within HTTPS are:

1. Authentication:

- SSL provides a mechanism for authenticating the identity of a website. When you visit a website using HTTPS, the server presents its SSL certificate, which is issued by a trusted Certificate Authority (CA).
- The browser checks this certificate to ensure it's valid and matches the website's domain. This helps users know they are connecting to the legitimate website and not a malicious one.

2. Encryption:

- SSL ensures that the data transmitted between a client (e.g., web browser) and the server is encrypted. This means that even if someone intercepts the data, they won't be able to understand it because it's in an unreadable form. This is crucial for protecting sensitive information like login credentials, personal data, and financial information.


- The purpose of encrypting traffic, especially for sensitive information like passwords or financial transactions, is to ensure that even if the data is intercepted by a malicious actor, they won't be able to make sense of it. Encryption scrambles the data into an unreadable format, and only the intended recipient (in this case, the server) has the key to decrypt it back into its original form.

## SSL Termination 
- refers to the process of decrypting the encrypted traffic at a specific point in the network infrastructure. This typically occurs at a load balancer or a proxy server before the traffic is forwarded to its final destination (like a web server). 
- Once the traffic is decrypted, it can be processed in its unencrypted form, potentially offloading computational work from the backend servers and improving overall system performance. This is particularly useful when a server or service behind the termination point doesn't need to deal with the overhead of SSL encryption/decryption, which can be computationally intensive.

