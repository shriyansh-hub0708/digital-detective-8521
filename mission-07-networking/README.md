
## Task 7.1 – Understanding Network Concepts

| Concept | Explain it in your own words | Example |
|---|---|---|
| LAN (Local Area Network) | A network that connects devices within a small geographical area. | Computers connected in a college laboratory. |
| MAN (Metropolitan Area Network) | A network that connects multiple LANs across a city or a large campus. | Networks connecting different college campuses in a city. |
| WAN (Wide Area Network) | A network that covers a large geographical area, such as multiple countries. | The Internet. |
| DNS (Domain Name System) | It translates a human-readable domain name into an IP address. | Finding the IP address of google.com. |
| Router | A networking device that connects different networks and forwards data between them. | A home Wi-Fi router connecting devices to the Internet. |
| Protocol | A set of rules that devices follow to communicate with each other. | HTTP, HTTPS and TCP/IP. |
| Packet Switching | A method in which data is divided into smaller packets before being transmitted across a network. | Sending a file over the Internet. |
| Client-Server | A communication model in which a client requests a service and a server provides it. | A phone requesting a video from YouTube. |

### What I Learned

Through this task, I learned about different types of networks and how devices communicate with each other. I understood the roles of DNS, routers and protocols, and how packet switching helps transfer data efficiently. I also learned how clients and servers work together to provide services over a network.


## Task 7.2 – Checking Network Connectivity and DNS

### 1. Checking Network Connectivity

I used the `ping` command in Terminal to check whether my computer could reach Google's server.

Command used:

```bash
ping -c 4 google.com
```

Result:
- 4 packets transmitted.
- 4 packets received.
- 0% packet loss.
- Average response time: 73.344 ms.

**Understanding:**

The ping command checks whether a destination can be reached over a network. It also measures the response time between my computer and the destination.

### 2. Performing a DNS Lookup

I used the `nslookup` command to find the IP addresses associated with Google's domain name.

Command used:

```bash
nslookup google.com
```

Result:
- DNS Server: 8.8.8.8
- Domain Name: google.com
- IP addresses returned included:
  - 142.251.126.101
  - 142.251.126.113
  - 142.251.126.139

**Understanding:**

The nslookup command queries a DNS server to find information about a domain name, such as its associated IP address.

### 3. Role of DNS When Opening a Website

When a user enters a website name such as google.com into a browser, DNS translates the human-readable domain name into an IP address. This allows the browser to locate the correct server and request the website.

### What I Learned

Through this task, I learned how to test network connectivity using the ping command and how to find the IP address of a domain using nslookup. I also understood how DNS helps browsers locate websites using domain names instead of requiring users to remember numerical IP addresses.


## Task 7.3 – What Happens When You Open a Website?

When a user enters a website name such as `google.com` into a browser, the following steps take place:

1. **Browser:** The user enters the website's domain name into the browser.
2. **DNS Lookup:** DNS translates the domain name into its corresponding IP address.
3. **Network Connection:** The computer uses its network connection and router to communicate with the destination server.
4. **Request:** The browser sends an HTTP or HTTPS request to the server asking for the website.
5. **Server Processing:** The server receives the request and prepares the required website content.
6. **Response:** The server sends the requested data back to the browser.
7. **Display:** The browser processes the received data and displays the website to the user.

### What I Learned

I learned how a browser, DNS, router, client and server work together when opening a website. I understood how DNS finds the server's IP address, how protocols help devices communicate, and how the server sends website data back to the browser.
