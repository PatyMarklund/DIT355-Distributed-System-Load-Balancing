# DIT355 - Distributed Systems - Load Balancing Repository

## Description
The Load Balancer component is one of four components of the DENS CURA system. The Load Balancer distributes work between 4 different backend services we call "Filters".  
Using LeastConn we can assign an API call to the Filter with least active connections/current requests via reverse proxying the request to our distributed systems.

For a more detailed view of the DENS CURA system, please view the [Main repository](https://github.com/PatyMarklund/DIT355-Distributed-System-Main).

## Installation
Clone project to local computer or server running Windows operating system.

## Usage
1. Start nginx.exe
2. If missing: Set all API calls from front-end to localhost:80 instead of localhost:3000  
    1. (In VS Code: ctrl + shift + F to search for "this.$http" to find all api calls in front-end)  
3. Start Filter as 4 different services with ports 3000, 3001, 3002, 3003
