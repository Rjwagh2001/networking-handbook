# Incident 05 — High Network Latency

## Scenario

An application is healthy but users experience elevated response times.

## Investigation checklist

- [ ] Establish baseline and affected time window.
- [ ] Compare application, network and dependency latency.
- [ ] Check packet loss and retransmissions.
- [ ] Inspect socket states and connection saturation.
- [ ] Check path MTU where relevant.
- [ ] Compare traffic paths and affected locations.

## Example tools

`mtr`, `ping`, `ss`, `tcpdump`, `tracepath`, application metrics and distributed traces.

## Evidence, root cause and resolution

_To be completed after the lab. Do not infer packet loss solely from an intermediate router failing to respond to ICMP._
