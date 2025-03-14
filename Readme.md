ansible-playbook -i inventory/hosts.ini general-k8s-setup.yml
ansible-playbook -i inventory/hosts.ini master-setup.yml
ansible-playbook -i inventory/hosts.ini worker-setup.yml