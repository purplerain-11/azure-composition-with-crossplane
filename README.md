How to Use the Playbook
Organize Your YAML Files:

Place all YAML files (get-azure-provider.yaml, provider-config.yaml, resource-group.yaml, virtual-network.yaml, virtual-machine.yaml) in the same directory or specify their path using the yaml_files_path variable.
Install Ansible and Dependencies:

Ensure Ansible is installed.
Install the Kubernetes Ansible collection:
bash
Copy
Edit
ansible-galaxy collection install kubernetes.core
Run the Playbook:

Execute the playbook:
bash
Copy
Edit
ansible-playbook crossplane_setup_with_yaml.yml
Notes
Order of Execution: The playbook ensures that each YAML file is applied in the correct sequence to avoid dependency issues.
Kubernetes Context: Ensure your Kubernetes context is set correctly to interact with the cluster running Crossplane.
Custom Paths: If your YAML files are not in the current directory, update the yaml_files_path variable with the correct path.
This playbook streamlines the process by leveraging your existing YAML definitions, making it easy to maintain and execute.
