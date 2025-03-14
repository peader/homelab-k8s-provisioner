- place the public ssh key from the master node into the worker nodes
echo -e "\n$USER ALL=(ALL) NOPASSWD: ALL\n" | sudo tee -a /etc/sudoers
ansible-playbook -i inventory/hosts.ini playbooks/general-k8s-setup.yaml
ansible-playbook -i inventory/hosts.ini playbooks/master-setup.yaml
ansible-playbook -i inventory/hosts.ini playbooks/worker-setup.yaml