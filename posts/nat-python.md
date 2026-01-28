# Understanding NAT with Python

In this post, I explore how NAT rewrites source IPs and ports using a simple Python client and server.

## The Problem
I wanted to see how my router rewrites traffic when sending requests to a remote server.

## The Experiment
I wrote two Python programs:
- a client that prints its internal IP and port
- a server that prints the public IP and NAT‑assigned port

## What I Learned
- My PC uses a private IP like `192.168.x.x`
- The server sees my router’s public IP instead
- The router rewrites the source port to keep connections unique

This helped me understand NAT in a very practical way.
