# ⚡Ansible Webserver Setup





## Introduction
This project automates the deployment of a web server using Ansible.
It installs and configures Nginx or Apache on remote servers and deploys a static HTML page.



## Architecture

- Control Node (Ansible): Machine where Ansible is installed and playbooks are executed.

- Inventory: Contains server connection details (IP, user, SSH key).

- Target Servers: Remote servers where the web server is installed and HTML page is deployed.
##  Installation

1. **Clone the repository:**  
```bash
git clone https://github.com/Nishika10/Ansible-webserver-setup.git
cd ansible-webserver-setup
```



## Deployment


1. Update inventory.ini with your server details:
 ```bash
[web_servers]
<server-ip> ansible_user=ubuntu ansible_ssh_private_key_file=/path/to/key.pem
```

2. Run the playbook:
```bash
ansible-playbook -i inventory.ini webserver_setup.yml
```

3. Verify by visiting the server IP in a browser.
##  Lessons
 
- Managing servers with Ansible.

- Automating service installation and configuration.

- Deploying files with Ansible modules.


  




## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.



## Author
**Nishika Jaiswal**

Aspiring Cloud & DevOps Engineer

