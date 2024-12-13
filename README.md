# LUM-Ansible: Linux User's Management

LUM-Ansible is an Ansible playbook that allows you to create and remove users on multiple remote servers. This playbook works only on Debian-based systems like Ubuntu, Parrot OS, Kali Linux, and other Debian-based systems.

## Features

- **Create multiple users** with sudo permissions.
- Assign **unique passwords** to each user.
- Automatically create a **home directory** for each user.
- Set up **SSH public key authentication** for secure login.
- Works seamlessly with **Debian-based systems** like Ubuntu, Parrot OS, and Kali Linux.
- And more...

### Components:
1. **Ansible Control Node**  
   - Runs the LUM-Ansible playbook.  
   - Connects to remote servers over SSH.  
   - Executes tasks like creating users, setting passwords, and configuring SSH keys.

2. **Remote Servers**  
   - Target Debian-based systems, such as:  
     - Ubuntu Server  
     - Parrot OS Server  
     - Kali Linux Server  
   - Receives user management tasks from the control node.

### Workflow:
1. The **Ansible Control Node** sends commands to the **Remote Servers** using the LUM-Ansible playbook.  
2. Tasks include user creation, setting permissions, password setup, and SSH key configuration.  
3. All changes are executed remotely and managed efficiently across multiple servers.

## Requirements

- Ansible installed on your control node.
- Target systems running a Debian-based Linux distribution.

## How to Use

Note: Create user's edit this **add_users.yml file and Remove user's edit this **rusers.yml file

1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/ATUL9372/LUM-Ansible.git

2. Run the Ansible playbook to create multiple users:
    ```bash
    ansible-playbook -i hosts create_users.yml

3. Run the Ansible playbook to remove multiple users:
    ```bash
    ansible-playbook -i hosts remove_users.yml


