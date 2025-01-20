# Crossplane Setup with Ansible Playbook

This guide explains how to set up Crossplane on Azure using an Ansible playbook. The playbook applies pre-defined Kubernetes YAML manifests for each step of the setup.

---

## How to Use the Playbook

### 1. Organize Your YAML Files

Ensure your YAML files are organized as follows:

```text
project-directory/
│
├── get-azure-provider.yaml
├── provider-config.yaml
├── resource-group.yaml
├── virtual-network.yaml
├── virtual-machine.yaml
└── crossplane_setup_with_yaml.yml  # The Ansible playbook
