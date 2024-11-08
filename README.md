# pinwheel-sde-intern-task

## Day 1
---
### Task 1: 

#### 1. **Entities and Properties**

Each node represents a key entity with properties relevant to cybersecurity.

| **Node Type**     | **Properties**                                                                                         |
|-------------------|--------------------------------------------------------------------------------------------------------|
| **Host**          | IP address, hostname, domain, OS, status (up, down), risk score                                        |
| **Port**          | Port number, protocol (TCP/UDP), state (open/closed/filtered)                                          |
| **Service**       | Service name (e.g., HTTP, SSH), version, protocol                                                      |
| **Vulnerability** | CVE ID, severity score, description, patch status                                                      |
| **Credential**    | Username, password hash, role (e.g., admin), hash algorithm                                            |
| **Exploit**       | Exploit name, type (e.g., SQL injection, buffer overflow), prerequisites, payload                      |
| **Operating System (OS)** | OS name, version, architecture (e.g., x86, x64), vulnerabilities                               |
| **File**          | File name, path, type (e.g., configuration, log), size, access rights                                  |
| **User**     | Username, privileges, role (e.g., user, admin), access rights                                         |
| **Tool**          | Tool name, purpose (e.g., scan, exploit), version, effectiveness                                      |


#### 2. **Relationships**

Each relationship type connects nodes to establish insights into the network, host vulnerabilities, potential exploits, and other security details.


| **Relationship**                   | **Description**                                                                                      |
|------------------------------------|------------------------------------------------------------------------------------------------------|
| **Host has Port**                  | Links a host to the specific ports that are open or closed on it.                                    |
| **Port runs Service**              | Connects a port to the service that is running on it.                                                |
| **Host runs Service**              | Indicates that a host is running a specific service.                                                 |
| **Host has Operating System**      | Specifies the operating system installed on the host.                                               |
| **Host has Vulnerability**         | Connects a host to vulnerabilities that are associated with it.                                      |
| **Vulnerability exploited by Exploit** | Links vulnerabilities to the exploits that can be used against them.                             |
| **Exploit used by Tool**           | Connects an exploit to the tool that can use or leverage it.                                         |
| **Tool used on Host**              | Indicates that a specific tool is used on a host, possibly for scanning or exploitation.             |
| **Vulnerability targets Host**     | Indicates that a vulnerability can potentially affect a host.                                        |
| **User has Host**                  | Connects a user to a host they own or have access to.                                                |
| **Host has File**                  | Indicates that a file is stored or found on a specific host.                                         |
| **Service needs Credentials**      | Connects a service to credentials required to access or use it.                                      |
| **Credentials give access to Host** | Links credentials to a host, indicating that they grant access to it.                               |

#### 3. **Graph**

![er](https://github.com/user-attachments/assets/1e59e08b-8424-4f87-969b-744e8378335b)


---
