# Hi, I'm Stepan 👋

**Tech Lead and Go engineer focused on Kubernetes platform engineering.**

I build controllers, operators, and runtime systems at the intersection of Kubernetes, Linux, cloud infrastructure, networking, and security. I enjoy turning complex lifecycle and reconciliation problems into predictable, observable systems.

<p>
  <img src="https://img.shields.io/badge/Go-00ADD8?logo=go&logoColor=white" alt="Go">
  <img src="https://img.shields.io/badge/Kubernetes-326CE5?logo=kubernetes&logoColor=white" alt="Kubernetes">
  <img src="https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black" alt="Linux">
  <img src="https://img.shields.io/badge/OpenStack-ED1944?logo=openstack&logoColor=white" alt="OpenStack">
</p>

## What I work on

- Architecture and development of Kubernetes controllers and operators in Go
- Dependency-aware scheduling, reconciliation loops, and lifecycle state machines
- Package and module management for Kubernetes platforms
- Cloud integrations, storage, networking, and workload orchestration
- Reliability, observability, and secure software delivery

## Deckhouse Kubernetes Platform

I currently work as a Tech Lead at [Flant](https://flant.com/) on [Deckhouse Kubernetes Platform](https://github.com/deckhouse/deckhouse).

My recent work includes:

- Leading the architecture of a unified package runtime for applications and modules
- Designing dependency-aware DAG schedulers with parallel execution and explicit lifecycle states
- Building reliable controller bootstrap, recovery, health monitoring, and finalizer-driven teardown
- Implementing integrity-protected OCI module delivery with EROFS and dm-verity
- Contributing to RBAC, multitenancy, ingress, CRD lifecycle, and platform observability

[Explore my Deckhouse contributions →](https://github.com/deckhouse/deckhouse/pulls?q=is%3Apr+author%3Aipaqsa)

## Managed Kubernetes on OpenStack

Previously, I worked on cloud's Managed Kubernetes service.

I helped design its next generation and migrate the control plane from Python to Go using custom controllers, an API service, and background workers. I also re-architected the CSI controller, Cloud Controller Manager, and cloud ingress controller for native integration with Nova, Neutron, Cinder, Octavia, and Keystone.

The platform managed cluster provisioning, deletion, node scaling, and Kubernetes upgrades, with idempotent reconciliation and retries for safe recovery from partial cloud failures.

## Technical interests

Kubernetes internals · Go · Linux · networking · distributed systems · system design · cloud computing · security

## Side project: kube2e

[kube2e](https://github.com/ipaqsa/kube2e) is a Go CLI for end-to-end testing of Kubernetes controllers, operators, Helm charts, and GitOps delivery.

Tests are written as declarative YAML and executed against a live cluster—no Go test code required. It supports Server-Side Apply, deterministic cleanup, retries, assertions, logs and exec checks, parallel execution, dry-run validation, machine-readable reports, and OCI-packaged test suites.

```bash
go install github.com/ipaqsa/kube2e/cmd/kube2e@latest
kube2e run ./examples --dry-run
```

[View kube2e on GitHub →](https://github.com/ipaqsa/kube2e)
