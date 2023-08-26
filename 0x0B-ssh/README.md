## SSH
- SSH stands for Secure Shell, and it is a network protocol used to securely access and manage remote servers and devices over a potentially unsecured network.
- SSH provides encrypted communication between a client and a server, ensuring that data transmitted between them remains confidential and cannot be easily intercepted by malicious actors.

- SSH allows users to log into a remote system and execute commands as if they were directly interacting with that system. It's commonly used for remote administration, file transfers, and secure access to servers and devices. 
- SSH operates by using a pair of cryptographic keys: 
	* a public key (stored on the server) and,
	* private key (stored on the client). 

- These keys are used to authenticate the client and establish a secure connection. SSH has largely replaced less secure remote access methods like Telnet and FTP (File Transfer Protocol).

## Creating an SSH RSA Key Pair:

1. Open a terminal on your local machine.

2. Use the ssh-keygen command to generate the RSA key pair:
```
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```

3. You'll be prompted to choose a location to save the key pair. The default is usually fine. Press Enter to confirm.

4. You'll be prompted to set a passphrase. This adds an extra layer of security. You can choose to set one or leave it blank for no passphrase. Press Enter after making your choice.

- This will generate two files in your chosen location: id_rsa (private key) and id_rsa.pub (public key).


## Connecting to a Remote Host Using an SSH RSA Key Pair:

1. Assuming you have the public key (id_rsa.pub), copy its contents to the remote server's ~/.ssh/authorized_keys file. You can do this manually or by using the ssh-copy-id command:
```
ssh-copy-id user@remote_host
```
Replace user with your username and remote_host with the remote server's address.


2. Once the public key is added to the authorized_keys file on the remote server, you can use the private key to connect:
```
ssh -i ~/.ssh/id_rsa user@remote_host
```

This command specifies the private key to use with the -i flag.
