##to run ansible playbook
ansible-playbook -i inventory.txt -u richardp update.yml --extra-vars="code_user="richardp""

## to run using tags
ansible-playbook -i inventory.txt -u richardp update.yml --extra-vars="code_user="richardp"" --tags bash_profile
ansible-playbook -i inventory.txt -u richardp update.yml --extra-vars="code_user="richardp"" --tags startup

##using shell global
ansible-playbook -i inventory.txt -u richardp update.yml --extra-vars="code_user="richardp"" --extra-vars="@deployment_vars/shell_global.yml"
