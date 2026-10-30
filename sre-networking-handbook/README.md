# SRE Networking Handbook

A practical, production-oriented networking learning journey for aspiring Site Reliability Engineers (SREs), DevOps Engineers, and Cloud Engineers.

The goal is not to complete a networking certification syllabus. The goal is to understand end-to-end request flows, build practical networking skills, troubleshoot production-style failures, and document the investigation process.

## Learning workflow

For each of the six selected learning sessions, follow this cycle:

1. **Watch** the session and take rough notes.
2. **Share** the concepts, commands, screenshots, and questions.
3. **Understand** the theory and how the technology works.
4. **Practice** through guided Linux, AWS, or Kubernetes labs.
5. **Troubleshoot** deliberately introduced failures.
6. **Document** the commands, expected results, observations, and fixes.
7. **Explain** the topic as if answering an SRE interview question.

> Do not copy commands without understanding them. Record what each command checks, what a healthy result looks like, and what an unexpected result means.

## Six-session roadmap

| # | Session | Main focus | Status |
|---|---|---|---|
| 01 | Networking fundamentals — Abhishek Veeramalla | OSI/TCP-IP, packets, IP addressing, CIDR, subnetting, routing | Not started |
| 02 | Linux networking — Linux Foundation session | Interfaces, routes, sockets, Linux diagnostics | Not started |
| 03 | Practical Networking | IP addressing, subnetting, routing and packet flow reinforcement | Not started |
| 04 | Cloudflare Learning Center | DNS, TCP, HTTP, HTTPS and TLS | Not started |
| 05 | AWS Networking Fundamentals | VPC, subnets, route tables, gateways, security and load balancing | Not started |
| 06 | Kubernetes networking — Linux Foundation session | Pod networking, CNI, Services, DNS, Ingress and NetworkPolicy | Not started |

The selected session links are collected in [`learning-resources.md`](learning-resources.md). Verify video availability and duration when starting each session.

## Repository structure

```text
sre-networking-handbook/
├── README.md
├── learning-resources.md
├── 01-networking-fundamentals/
│   ├── README.md
│   ├── theory.md
│   ├── practical-labs.md
│   └── troubleshooting.md
├── 02-linux-networking/
│   ├── README.md
│   ├── theory.md
│   ├── practical-labs.md
│   └── troubleshooting.md
├── 03-ip-addressing-subnetting/
│   └── README.md
├── 04-dns-tcp-http-tls/
│   └── README.md
├── 05-aws-networking/
│   └── README.md
├── 06-kubernetes-networking/
│   └── README.md
├── production-incidents/
│   ├── README.md
│   ├── incident-01-application-timeout.md
│   ├── incident-02-database-connectivity.md
│   ├── incident-03-kubernetes-service-failure.md
│   ├── incident-04-dns-resolution-failure.md
│   └── incident-05-high-network-latency.md
└── images/
    └── README.md
```

## Recommended study routine

Target: **2 hours per study day**.

| Time | Activity |
|---:|---|
| 30 minutes | Watch the selected video |
| 30 minutes | Review concepts and write notes |
| 45 minutes | Perform a practical lab |
| 15 minutes | Explain the learning and answer interview questions |

Use this as a guide, not a rigid rule. Some labs may need more time. Prioritize safe, repeatable understanding over rushing.

## Documentation standard for every topic

For each concept or lab, document:

1. **What** — definition and purpose.
2. **Why** — why production systems use it.
3. **How** — how it works, including the request or packet flow.
4. **Where** — which layer or component is involved.
5. **Commands** — commands used and what each one checks.
6. **Expected result** — what a healthy result looks like.
7. **Troubleshooting** — common symptoms and diagnostic steps.
8. **Production relevance** — a realistic SRE scenario.
9. **Resolution** — root cause, mitigation and permanent fix.
10. **Interview explanation** — a concise explanation in your own words.

## Important safety notes

- Run labs only on systems and networks you own or are explicitly authorized to test.
- Prefer a disposable lab VM or local Minikube cluster for failure simulations.
- Do not run disruptive firewall, routing, packet-loss, or network-policy experiments on production systems.
- Avoid publishing credentials, private keys, public IPs that should remain private, account IDs, tokens, or sensitive configuration in Git.
- Review command output before committing it; redact sensitive details.

## Progress checklist

- [ ] Session 01 — Networking fundamentals
- [ ] Session 02 — Linux networking
- [ ] Session 03 — IP addressing and subnetting
- [ ] Session 04 — DNS, TCP, HTTP and TLS
- [ ] Session 05 — AWS networking
- [ ] Session 06 — Kubernetes networking
- [ ] Complete five production-style incident exercises
- [ ] Complete the end-to-end networking capstone

## Capstone project: Production Network Troubleshooting Lab

Build a small, controlled environment that demonstrates:

- A Linux host and basic IP routing.
- An application exposed through a Kubernetes Service and Ingress.
- DNS lookup and HTTP/TLS connectivity checks.
- AWS VPC networking concepts, documented through an architecture and (when available) a safe lab.
- Monitoring and evidence collection for connectivity, latency, and service health.

Simulate and investigate failures such as:

- Incorrect DNS configuration.
- Blocked application port.
- Incorrect Kubernetes Service selector or `targetPort`.
- Unhealthy load-balancer target.
- Restrictive NetworkPolicy.
- Increased latency or packet loss in a controlled environment.

For every incident, capture the symptom, impact, investigation, evidence, root cause, mitigation, permanent fix, and prevention.

## Definition of done

The learning journey is complete when you can:

- Trace a request from a client to an application and its backend.
- Explain the relevant OSI/TCP-IP layers without treating them as a literal execution pipeline.
- Diagnose DNS, routing, TCP, port, TLS, load-balancer, and Kubernetes Service issues.
- Use Linux networking tools and interpret their output.
- Explain AWS VPC and Kubernetes networking fundamentals.
- Write clear incident reports and explain your troubleshooting decisions.

---

**Learning principle:** Understand → Practice → Break safely → Troubleshoot → Document → Explain.
