# holbertonschool-network
## What is localhost/127.0.0.1
"localhost" and "127.0.0.1" are both references to the loopback IP address of a computer or network interface. When used, they typically refer to the local machine itself.

Here's what each of them means:
### localhost:
It is a hostname that represents the current device used to access it. In simple terms, when you type "localhost" into a web browser or use it in a network application, it refers to the machine you are using at that moment. It is often used to access the web server software installed on the same device for testing and development purposes.
### 127.0.0.1: 
 This is the numerical IP address associated with the localhost hostname. It is a special IP address reserved for loopback testing purposes. When you use "127.0.0.1" as an IP address, you are specifically targeting the loopback interface of your own device. Any network requests made to this IP address are directed back to the same device without going through any network communication.

Both "localhost" and "127.0.0.1" are commonly used in web development, server configurations, and network troubleshooting to test or access services running on the local machine without involving external network traffic.
## What is localhost/127.0.0.1 :
The IP address "0.0.0.0" is a special address used to represent an invalid, unknown, or unspecified target in networking contexts. It has different meanings depending on the context in which it is used:
### Default route or default gateway :
In the context of network routing, "0.0.0.0" is often used as the default route or default gateway. It indicates that all network traffic destined for an unknown or unspecified IP address should be sent to the default gateway for further routing. In other words, when a device doesn't have a specific route for a given IP address, it uses the default route as a fallback.
### Binding to all available network interfaces :
 In some network applications or server configurations, specifying "0.0.0.0" as the IP address means to bind or listen on all available network interfaces of the device. It allows the application or server to accept connections from any IP address that the device may have, including localhost (127.0.0.1) and any externally accessible IP addresses.

 In summary, "0.0.0.0" is used to represent an unspecified or all IP addresses depending on the context. It serves as the default route or default gateway in networking, and it can also be used to bind to all available network interfaces in server configurations.
## What is /etc/hosts:
The "/etc/hosts" file is a plain text file commonly found in Unix-like operating systems, including Linux and macOS. It is used to map hostnames to IP addresses on a local machine, allowing the operating system to resolve domain names without the need for external DNS (Domain Name System) lookups.

- Each line in the "/etc/hosts" file typically contains an IP address followed by one or more hostnames associated with that IP address. The format is as follows:
                        <IP address>   <hostname1> <hostname2> ...
- For example:
                        127.0.0.1       localhost
                        192.168.0.10    myserver
- In the above example, "localhost" is mapped to the loopback IP address 127.0.0.1, and "myserver" is mapped to the IP address 192.168.0.10.
- When a program or the operating system attempts to resolve a hostname, it first checks the "/etc/hosts" file to see if there is an entry for that hostname. If a match is found, the corresponding IP address is used for communication. If there is no match, the system proceeds with DNS resolution to find the IP address associated with the hostname.
- The "/etc/hosts" file is often used for local network configuration, testing, or development purposes, allowing users to define custom mappings of hostnames to IP addresses without relying on external DNS servers.

## How to display your machine’s active network interfaces:
To display the active network interfaces on your machine, you can use various commands depending on your operating system. Here are the commands for different operating systems:
*  Linux: You can use the ifconfig command or the newer ip command to display active network interfaces. Open a terminal and enter one of the following commands:
                            ifconfig
-or 
                            ip addr show
The output will list the active network interfaces along with their respective IP addresses, MAC addresses, and other details.