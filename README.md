# SpartanRPC

This distributed RPC framework is developed based on Golang 's standard library net/rpc.

Spartan RPC is a lightweight Golang-based distributed remote procedure call(RPC) framework that can efficiently connect different services in and across the system to reduce redundant work in the communication routines with extra support in timeout handling, services load balancing and monitoring for edge devices that have limited computing capacity. It is built on top of the Golang net/rpc library and includes all the basic functionality that the library provides:
JSON-based efficient request encoding and response decoding, data serialization and deserialization
Server-side server initialization and hosting, service and method registration, RPC request receiving and processing, and RPC response sending 
Client-side client initialization and connecting, RPC procedure asynchrony and concurrency, RPC request sending and RPC response receiving



More importantly, advanced features were designed and implemented to better support different needs of an edge device in edge computing or distributed computing environment that uses RPC:
RPC timeout handling mechanism to ensure the call is regulated by customized timeout value for connection time and processing time  
HTTP protocol exchange to support HTTP-based web service utilization
Load balancing utility through random selection and Round Robin scheduling algorithm to dynamically regular the overall loads of each server
RPC registry that supports service registration, discovery, and heartbeat monitoring to support distributed system computing environment

