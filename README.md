##to run ansible playbook
ansible-playbook -i inventory.txt -u richardp update.yml --extra-vars="code_user="richardp""

## to run using tags
ansible-playbook -i inventory.txt -u richardp update.yml --extra-vars="code_user="richardp"" --tags bash_profile
ansible-playbook -i inventory.txt -u richardp update.yml --extra-vars="code_user="richardp"" --tags startup
