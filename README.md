# Turret - Just a smaller Tower

Turret distributes Ansible® execution with a simple API and minimal set of requirements.

## Why

There is a gap between the simplicity of CLI Ansible and the full featured Ansible Tower®/AWX. We think, Turret can fulfill this gap by keeping the simplicity. The idea behind Turret was to run Ansible as a backend application.

To use Turret for:

- Use Ansible as backend service
- Execute Ansible by CI/CD pipelines
- Centralized API but distributed Ansible workload

## Why not

Because Turret should never compete with Ansible Tower®/AWX, these are non-goals:

- Full blown user-friendly UI
- User management
- Role based access control
- Inventory management

## Requirements

While simplicity is the main goal, scaling Ansible is the side goal. Turret can run Ansible on a single host but also uses existing infra, such as Kubernetes, Hashicorp Nomad® or Apache Mesos to scale Ansible execution.

Currently, a PoC exists with the following minimal requirements:

- A RDBMS (SQlite, MySQL, PostgreSQL)
- Redis (Queue)
- 1 Dockerhost (or alternatively Kubernetes/Openshift Cluster)

## License / Trademarks

Affero General Public License (AGPLv3). Ansible® and Ansible Tower® is a registered trademark of Red Hat®.
