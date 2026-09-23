# Hi, I'm Stepan 👋

**Tech Lead and Go engineer focused on Kubernetes platform engineering.**

I develop Kubernetes platform software in Go. My work includes controllers and operators, package management, dependency scheduling, and cloud integration, with a focus on keeping production systems reliable during upgrades, failures, and configuration changes.

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

Selected work:

- **Unified package runtime:** led the architecture and implementation of a shared runtime for applications and modules, based on declarative Kubernetes controllers. [#21857](https://github.com/deckhouse/deckhouse/pull/21857) [#21997](https://github.com/deckhouse/deckhouse/pull/21997)
- **Dependency-aware scheduling:** designed schedulers with critical/functional isolation, parallel execution, topological ordering, and explicit lifecycle states. [#13906](https://github.com/deckhouse/deckhouse/pull/13906) [#18121](https://github.com/deckhouse/deckhouse/pull/18121)
- **Secure module delivery:** implemented read-only OCI module delivery using EROFS and dm-verity, with integrity and signature verification. [#15019](https://github.com/deckhouse/deckhouse/pull/15019) [#15450](https://github.com/deckhouse/deckhouse/pull/15450)
- **RBAC and multitenancy:** developed core parts of RBAC v2 and project reconciliation for namespace- and cluster-scoped administration. [#8538](https://github.com/deckhouse/deckhouse/pull/8538) [#9291](https://github.com/deckhouse/deckhouse/pull/9291)
- **Platform reliability:** built package health monitoring and safe finalizer-driven resource teardown. [#19711](https://github.com/deckhouse/deckhouse/pull/19711) [#22372](https://github.com/deckhouse/deckhouse/pull/22372)

[Explore my Deckhouse contributions →](https://github.com/deckhouse/deckhouse/pulls?q=is%3Apr+author%3Aipaqsa)

## Upstream open-source contributions

I also contribute fixes and features upstream to projects used by the Kubernetes ecosystem:

- **Helm:** added support for custom Go template functions when Helm is embedded as a library. [helm/helm#30734](https://github.com/helm/helm/pull/30734)
- **ingress-nginx:** added HTTP/3 support with NGINX 1.25.5, documented its configuration, and fixed temporary NGINX configuration cleanup. [#11470](https://github.com/kubernetes/ingress-nginx/pull/11470) [#11513](https://github.com/kubernetes/ingress-nginx/pull/11513) [#11569](https://github.com/kubernetes/ingress-nginx/pull/11569)
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
