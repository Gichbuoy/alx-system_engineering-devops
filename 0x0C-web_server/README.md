
## Main Role of a Web Server:
- The main role of a web server is to respond to incoming HTTP (Hypertext Transfer Protocol) requests from clients, typically web browsers, by delivering web content such as HTML files, images, videos, and other resources.
- It handles the communication between the client and the server, ensuring that the requested content is retrieved and sent back to the client in a timely and efficient manner. 
- Web servers also manage security, authentication, and sometimes perform other tasks like dynamic content generation through server-side scripting.

## Parent and Child Processes in Web Servers:
- Web servers often utilize a parent-child process model for managing incoming client requests. 
- The parent process is responsible for accepting incoming connections and managing the creation of child processes to handle those connections. Each child process is dedicated to serving a specific client request, allowing multiple requests to be handled simultaneously in a concurrent manner. This architecture helps improve performance and responsiveness by distributing the workload across multiple processes.

## DNS
-> DNS stands for Domain Name System.

- The main role of DNS is to translate human-readable domain names, like "www.example.com," into IP addresses that computers and network devices use to identify each other on the internet. 
- In essence, DNS acts as a directory service for the internet, allowing users to access websites and other online resources using easy-to-remember domain names instead of having to remember the numeric IP addresses associated with those resources.

- DNS achieves this by maintaining a distributed database that contains records mapping domain names to their corresponding IP addresses. 
- When a user enters a domain name into a web browser or clicks a link, the browser contacts a DNS resolver (typically provided by the user's internet service provider) to resolve the domain name to an IP address. The resolver then communicates with DNS servers to find the appropriate IP address for the given domain. Once the IP address is obtained, the browser can connect to the web server associated with that IP to retrieve the requested content.

## DNS Record Types
1. A (Address) Record:
- An A record maps a domain name to an IPv4 address. It is used to resolve a domain name to the corresponding IP address. For example, if you have an A record for "www.example.com," it points to the specific IPv4 address where the website is hosted.

2. CNAME (Canonical Name) Record:
- A CNAME record is used to create an alias for a domain name. It points one domain name to another domain name rather than to an IP address. This is often used for subdomains or when you want multiple domain names to resolve to the same IP address. For instance, if you have a CNAME record for "blog.example.com" pointing to "www.example.com," both URLs will resolve to the same content.

3. TXT (Text) Record:
- A TXT record is used to store arbitrary text data associated with a domain. It is commonly used for various purposes, such as domain verification, SPF (Sender Policy Framework) records for email authentication, and other forms of human-readable information. For example, TXT records are used to specify SPF policies to prevent email spoofing.

4. MX (Mail Exchange) Record:
- An MX record specifies the mail servers responsible for receiving email messages destined for a domain. It associates a domain name with a list of mail servers' hostnames or IP addresses, along with a priority value to determine the order in which servers should be used for mail delivery. This record is crucial for email communication, as it directs incoming emails to the appropriate mail servers.

