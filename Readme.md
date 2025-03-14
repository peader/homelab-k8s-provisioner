ansible-playbook -i inventory/hosts.ini playbooks/general-k8s-setup.yaml
ansible-playbook -i inventory/hosts.ini playbooks/master-setup.yaml
ansible-playbook -i inventory/hosts.ini playbooks/worker-setup.yaml