# Ansible prometheus-node-exporter

Ansible role to install and configure Prometheus node-exporter.

## Requirements

None.

## Role Variables

See defaults/main.yml for details

## Dependencies

None.

## Install this role as submodule in a git repository

```sh
git submodule add https://git.sekoya.org/mb/ansible_prometheus_node_exporter.git roles/prometheus-node-exporter
```

## Example Playbook

    - hosts: servers
      roles:
        - prometheus-node-exporter


    - hosts: servers
      roles:
        - role: prometheus-node-exporter
          prometheus_node_exporter_defaults:
            - --web.listen-address=10.0.0.1:9100

## License

GPLv3

## Author Information

https://www.sekoya.org
