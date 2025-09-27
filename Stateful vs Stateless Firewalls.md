# Stateful vs. Stateless Firewalls

## Stateful Firewalls:

Tracks the state of active network connections and remembers previous packets in a session.

- Maintains a "state table" that records details about active connections.

- Stronger than stateless firewalls and more secure. In AWS, it implicitly denies all traffic that isnt explicitly allowed.

- More compute heavy so requires more processing power and memory and therefore can add latency and higher costs.

## Stateless Firewalls:

Evaluates each network packet in isolation without any memory of previous packets in a connection.

- Uses a static Access Control List (ACL) to either allow/deny traffic based on source/destination IP Addresses, Port numbers, and protocols.

- Less secure than stateful firewalls. Cannot detect attacks whereas stateful firewalls can.

- Processes packets quicker and more efficiently because it requires less compute power. Less latency.

- Requires specific rules for both inbound and outbound traffic.

## TCP and IP Refresher

Transmission Control Protocol is when you make a connection using TCP, what is actually happening is that each side (client and server) is sending IP packets to each other. These packets have a source and destination IP address and are carried across the local network and the public internet.

- Clients usually have random port numbers whereas servers typically have "well known" ports

- HTTP = Port 80 (Well known)
-HTTPS = Port 443. (Well known)