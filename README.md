# log4shell-detector Playbook

This simple Ansible Playbook can be used to clone and execute the [log4shell-detector](https://github.com/Neo23x0/log4shell-detector) pyhon script to detect CVE-2021-44228 exploit attempts in your infrastructure.

The playbook will save the findings for each host under **reports/{hostname}**

## Instructions

Clone the repository.

```sh
git clone https://github.com/kaipee/log4shell-detector-playbook.git
```

Create your inventory file.

```sh
cd log4shell-detector-playbook
touch inventory
```

Add your host entries to the inventory file.


Run the playbook.

```sh
ansible-playbook -i inventory main.yml
```

Review the findings for each host under the **reports** directory.

## Credits

All credit goes to [@cyberops](https://twitter.com/cyb3rops) for the log4shell-detector tool.
