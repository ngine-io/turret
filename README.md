# Turret - Just a smaller Tower

Turret distributes Ansible® execution with a simple API and minimal set of requirements.

## Why

There is a gap between the simplicty of CLI ansible and the full featured Ansible Tower®/AWX. We think, Turret can fullfil this gap by keeping the simpliticy. The idea behind Turret was to run Ansible as a backend application.

To use Turret for:

- Use Ansible as backend service
- Execute Ansible by CI/CD pipelines
- Centralized API but distributed Ansible workload

## Why not

Because Turret should never compete with Ansible Tower®/AWX, these are non-goals:

- Full blown user friendly UI
- User management
- Role based access control
- Inventory management

## Requirements

While simplitcy is main goal, scaling Ansible is the side goal. Turret can run Ansible on a simgle host but also use exisitng infra, such as Kubernetes, Hashicorp Nomad® or Apache Mesos to scale Ansible execution.

Currently a PoC existis with the follwoing minimal requirements:

- A RDBMS (SQlite, MySQL, PostgreSQL)
- Redis (Queue)
- 1 Dockerhost (or alternatively Kubernetes/Openshift Cluster)

## License / Trademarks

Affero General Public License (AGPLv3). Ansible® and Ansible Tower® is a registered trademark of Red Hat®.
