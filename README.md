
# LISP-Mobility
Cisco LISP-Mobility LAB
LISP Lab Setup Guide
Overview
This lab demonstrates Locator/ID Separation Protocol (LISP) implementation with the following topology:

MS-MR (Map Server/Map Resolver): Central LISP infrastructure component
XTR-1: LISP xTR (Ingress/Egress Tunnel Router) with EID subnet
XTR-2: Standard router for connectivity testing
VRF-Test Router: Client device for testing LISP mobility

Network Architecture
                    MS-MR (3.3.3.3)
                   /              \
                  /                \
           XTR-1 (1.1.1.1)    XTR-2 (2.2.2.2)
                |                   |
                 EID: 172.16.10.0/24   
Key LISP Concepts

EID (Endpoint Identifier): 172.16.10.0/24 - The mobile subnet
RLOC (Routing Locator): Loopback addresses of routers
Map Server/Resolver: Central database for EID-to-RLOC mappings
xTR: Performs LISP encapsulation/decapsulation

Lab Objectives

Configure LISP Map Server and Map Resolver
Set up LISP xTR functionality
Test EID mobility and reachability
Understand LISP encapsulation process

Prerequisites

Basic understanding of IP routing and OSPF
Familiarity with Cisco IOS configuration
CSR1000v routers or similar LISP-capable devices
