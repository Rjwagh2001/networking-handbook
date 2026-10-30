# Networking Fundamentals — Practical Labs

Run these exercises on a Linux lab machine or another system you are authorized to inspect. Commands are diagnostic and generally read-only.

## Lab 1 — Inspect network interfaces and addresses

```bash
ip addr
ip link
```

Record:
- Interface names.
- Interface state.
- IPv4/IPv6 addresses.
- MAC address.

## Lab 2 — Inspect the routing table

```bash
ip route
ip route get 8.8.8.8
```

Record:
- Default route.
- Gateway address.
- Interface selected for the destination.

## Lab 3 — Inspect the neighbour table

```bash
ip neigh
```

Explain what a neighbour entry represents and how it relates to ARP on IPv4.

## Lab 4 — Test basic connectivity

```bash
ping -c 4 8.8.8.8
```

Then compare with:

```bash
ping -c 4 google.com
```

Explain why these two tests check different parts of the path. A failed ping does not by itself prove that a service is unavailable; ICMP may be filtered.

## Lab record template

For each lab, record:

- **Objective:**
- **Environment:**
- **Commands:**
- **Expected result:**
- **Actual result:**
- **What I learned:**
- **Troubleshooting notes:**
- **Screenshot or sanitized output:**
