# ADD-ON — FREE COMPUTER / ENGINEERING ROADMAP

## QUICK START

I use one main resource per stage, official documentation as reference, and a project as the gate.

I do not collect courses.

## 1. COMPUTER + CS FOUNDATION

Primary:

- Harvard CS50x: https://cs50.harvard.edu/x/

Use it to build general computing/programming foundations.

Supplement:

- MIT Missing Semester: https://missing.csail.mit.edu/

Use it for shell, command-line tools, Git, editors and practical computing.

## 2. LINUX / SHELL

- Linux man pages
- GNU/Linux documentation
- MIT Missing Semester

Gate:

Create users/files/permissions, inspect processes, services, logs, disks and networking from the terminal.

## 3. GIT

- Pro Git: https://git-scm.com/book/en/v2

Gate:

clone → branch → edit → commit → merge/rebase basics → remote → inspect history → resolve a conflict.

## 4. PYTHON

- Python documentation: https://docs.python.org/3/
- CS50 Python: https://cs50.harvard.edu/python/

Gate:

Write a useful script without following a tutorial line-by-line.

## 5. NETWORKING

Study:

- IP/CIDR
- DNS
- DHCP
- ARP
- TCP/UDP
- ports
- routing
- NAT
- HTTP/HTTPS
- TLS
- SSH
- firewalls

Use practical Linux tools:

ip, ss, ping, traceroute/tracepath, dig, curl, ssh.

Gate:

Given “the application cannot connect”, investigate layer by layer instead of randomly restarting things.

## 6. SQL / POSTGRESQL

Official tutorial:

https://www.postgresql.org/docs/current/tutorial.html

Gate:

Design a small schema, use constraints, joins, aggregation, indexes and transactions, then explain why a query works.

## 7. WEB / HTTP

MDN Learn:

https://developer.mozilla.org/en-US/docs/Learn_web_development

Gate:

Explain browser → DNS → TCP/TLS → HTTP request → application → database → response.

## 8. FASTAPI

Official tutorial:

https://fastapi.tiangolo.com/tutorial/

Gate:

Build, test, validate and document a small API connected to PostgreSQL.

## 9. DOCKER

Official getting started:

https://docs.docker.com/get-started/

Gate:

Build an image, run a container, configure a network/volume, inspect logs, use Compose and diagnose a broken service.

## 10. AWS

Use AWS's current training material:

https://skillbuilder.aws/

Start with fundamentals before specializing.

Gate:

Deploy and explain a small architecture and its security/networking choices.

## 11. TERRAFORM

Official tutorials:

https://developer.hashicorp.com/terraform/tutorials

Gate:

Provision, inspect, change and destroy reproducible infrastructure.

## 12. CI/CD

Start with GitHub Actions documentation:

https://docs.github.com/actions

Gate:

push code → automated checks → artifact/build → controlled deployment.

## 13. OBSERVABILITY

Learn:

- logs
- metrics
- traces
- alerting
- SLIs/SLOs
- incident investigation

Gate:

Find the cause of a deliberately introduced failure using telemetry.

## 14. KUBERNETES

Official basics:

https://kubernetes.io/docs/tutorials/kubernetes-basics/

Gate:

deploy → inspect → scale → break → recover → explain.

## 15. AI SYSTEMS

Only after the systems foundation is real.

Study:

- model APIs
- embeddings
- RAG
- vector search
- evaluation
- serving
- AI infrastructure/MLOps
- production integration

The point is to become the engineer who can make AI systems work in the real world, not just call an API.

## RESOURCE RULE

For every stage:

**one primary resource + official docs + one project + one gate.**

If I need five courses to understand one topic, the problem may be my foundation, not the lack of courses.

Last reviewed: 2026-09-25
