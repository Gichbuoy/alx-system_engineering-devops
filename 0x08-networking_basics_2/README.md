## Networking Basics_2

### Locahhost
- "Localhost" refers to the loopback network interface of a device
- When a device accesses "localhost," it is referring to itself.
- It is often used for testing and running applications locally without the need for an internet or network connection.

### Hosts file
- The hosts file is a simple text file found on most operating systems.
- Used to map hostnames to corresponding IP addresses before querying a DNS (Domain Name System) server.

- The hosts file allows local, manual resolution of domain names without relying solely on DNS.

- When a device wants to access a specific hostname, it first checks the hosts file to see if there is a mapping for that hostname. If a matching entry is found in the hosts file, the device uses the associated IP address for communication. If there is no matching entry, the device proceeds to query a DNS server to resolve the hostname.


- The hosts file can be manually edited to add or modify entries. It is often used for various purposes, such as:

* Local development and testing: Developers can use the hosts file to map domain names to local IP addresses, allowing them to test websites or applications on their own machines before making them publicly accessible.

* Blocking or redirecting websites: By mapping unwanted domain names to a non-functional IP address (e.g., 0.0.0.0), users can block or redirect access to specific websites.

* Network customization: Network administrators can use the hosts file to enforce custom mappings for internal resources or override public DNS resolutions.
