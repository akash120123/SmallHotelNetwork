Introduction

The Small Hotel Network Project aims to create a reliable and efficient networking infrastructure for a three-story hotel. By implementing a structured approach that utilizes VLANs for network segmentation, OSPF for dynamic routing, and DHCP for automatic IP address allocation, this project ensures that all departments can communicate effectively while maintaining high security and performance standards. This network design accommodates various departments, including Reception, Finance, IT, and more, providing seamless connectivity and robust access to resources, such as printers and Wi-Fi, throughout the hotel.

Project Details

Number of Floors : 3
Departments:
  - 1st Floor: Reception, Store, Logistics
  - 2nd Floor: Finance, HR, Sales/Marketing
  - 3rd Floor: IT, Admin

Network Design

- Routers: Three routers located in the IT department, connected via serial DCE cables.
- Switches: Each floor is equipped with one switch to facilitate wired connections.
- Wireless Access: Wi-Fi networks available for laptops and mobile devices in each department.

Routing Protocol
- The network employs OSPF (Open Shortest Path First) as the routing protocol to efficiently advertise routes between the routers.

DHCP Configuration
- Each router is configured as a DHCP server, enabling devices to obtain IP addresses dynamically, streamlining network management.

Security Measures

- SSH Configuration**: SSH is set up on all routers for secure remote login.
- Port Security: The IT department switch implements port security to allow only the designated Test-PC to access port fa0/1, utilizing sticky MAC address learning with a violation mode of shutdown for enhanced security.

Testing and Validation
- A PC, named Test-PC, is connected to port fa0/1 in the IT department for testing remote login functionality.
- Comprehensive testing ensures that all devices can communicate effectively within the network.
