# ee-console

AtGlance is a self-hosted operations platform that connects an Ubuntu‑focused CLI agent with a central management console to make service operations safer, traceable, and easier to automate for engineering teams.

The CLI runs on Linux/systemd hosts and gives operators a single entry point to:

- Discover systemd services, ports, and recent log signal health.
- Classify service health with deterministic rules (working, warning, error, restarting, etc.).
- Manage configuration lifecycle: save, list, upload, and import service configuration backups with local fallback and remote version history.
- Manage system lifecycle: register hosts, validate access, deregister on decommission, and reactivate inactive systems.

The AtGlance Management Console is a Application + Kong + Database + Redis stack that organizations deploy inside their own network boundary. It provides:

- RBAC driven dashboards for superadmin, admin, and user roles.
- Central views for systems, services, configuration versions, and activity logs.
- PAT‑token secured APIs for system/CLI integrations.
- Resilient write behavior using Redis backed queues and a database circuit breaker so API writes are queued and replayed on DB recovery.

**Key features**

- Self-hosted, on‑prem / private‑cloud friendly.
- CLI + Web UI designed for SREs, platform teams, and DevOps.
- Configuration versioning with local and remote backups.
- System registration and governance with workspace/org scoping.
- Optional S3 storage and migration from local storage.
- SSO‑ready (GitHub implemented, additional providers planned).

See the docs and architecture diagrams in this repo for end-to-end flows, CLI flags, and API endpoints.
