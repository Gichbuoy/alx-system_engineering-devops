
## Main Role of a Web Server:
- The main role of a web server is to respond to incoming HTTP (Hypertext Transfer Protocol) requests from clients, typically web browsers, by delivering web content such as HTML files, images, videos, and other resources.
- It handles the communication between the client and the server, ensuring that the requested content is retrieved and sent back to the client in a timely and efficient manner. 
- Web servers also manage security, authentication, and sometimes perform other tasks like dynamic content generation through server-side scripting.

## Parent and Child Processes in Web Servers:
- Web servers often utilize a parent-child process model for managing incoming client requests. 
- The parent process is responsible for accepting incoming connections and managing the creation of child processes to handle those connections. Each child process is dedicated to serving a specific client request, allowing multiple requests to be handled simultaneously in a concurrent manner. This architecture helps improve performance and responsiveness by distributing the workload across multiple processes.

