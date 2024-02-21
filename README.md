# Default Outbound Access virtual machine nic checker
This repository contains a KQL query for checking Azure virtual machine NICs for default outbound access.
The query will first fetch all virtual machine network interface (NIC) resources in the selected scope. It will then check if that NIC has a public IP address assignment, is part of a public Azure load balancer backend pool, is in a subnet assigned to a NAT gateway or is in a subnet that has a default route with a next hop type of virtual appliance.

There is also a JSON file which you can import into an Azure workbook for a better visual representation on the query results.
