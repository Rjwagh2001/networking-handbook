# Incident 03 — Kubernetes Service Failure

## Scenario

A client cannot reach an application through a Kubernetes Service.

## Investigation checklist

- [ ] Check Pod readiness and restart counts.
- [ ] Inspect Service selector and ports.
- [ ] Inspect EndpointSlices.
- [ ] Verify application listens on the expected interface and port.
- [ ] Check NetworkPolicy and CNI health.
- [ ] Test DNS and connectivity from a temporary diagnostic Pod.

## Example commands

```bash
kubectl get pods -o wide
kubectl get svc
kubectl describe svc <service-name>
kubectl get endpointslices
kubectl get networkpolicy
```

## Evidence, root cause and resolution

_To be completed after the lab._
