# Incident 04 — DNS Resolution Failure

## Scenario

A client or Pod cannot resolve a service hostname.

## Investigation checklist

- [ ] Identify the exact hostname and expected answer.
- [ ] Check resolver configuration.
- [ ] Query the configured resolver.
- [ ] Compare with an authoritative or approved alternate resolver where appropriate.
- [ ] Check record type, TTL and recent changes.
- [ ] For Kubernetes, inspect CoreDNS Pods, logs and service configuration.

## Example commands

```bash
dig <hostname>
nslookup <hostname>
cat /etc/resolv.conf
```

## Evidence, root cause and resolution

_To be completed after the lab._
