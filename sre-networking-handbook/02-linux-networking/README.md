# 02 — Linux Networking

**Learning session:** Linux Foundation practical troubleshooting session.

## Objectives

- Inspect interfaces, addresses and routes.
- Inspect listening ports and active sockets.
- Test DNS and TCP connectivity.
- Understand basic packet capture with `tcpdump`.
- Build a repeatable Linux network troubleshooting sequence.

## Planned commands

```bash
ip addr
ip link
ip route
ip neigh
ss -tulnp
ss -ant
dig example.com
curl -v https://example.com
nc -vz example.com 443
tcpdump -i any
traceroute example.com
mtr example.com
```

Use only commands installed on your lab system. Some commands may require installation or elevated privileges.

## Completion checklist

- [ ] Watch Session 02.
- [ ] Explain each command and its output.
- [ ] Complete guided labs.
- [ ] Document one connectivity failure and its diagnosis.
