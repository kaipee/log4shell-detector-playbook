# log4shell-detector Playbook

This simple Ansible Playbook can be used to clone and execute the `log4shell-detector` pyhon script to detect CVE-2021-44228 exploit attempts in your infrastructure.

The playbook will save the findings for each host under **reports/{hostname}**

## How to

Clone the repository.

```sh
git clone https://github.com/kaipee/log4shell-detector-playbook.git
```

Create your inventory file.

```sh
cd log4shell-detector-playbook
touch inventory
# Add your host entries
```

Run the playbook.

```sh
ansible-playbook -i inventory main.yml
```
