      Cisco IOS, IOS-XE configuration with Ansible
 
- Execute one of the tree playbook in the top of the directory tree. 
- Each file include different static configuration and options controlled with variables in
*_var files. Jinja2 templates are stored into role/templates directory.
- Variable files include nonstatic configuration and configuration of network protocols,
such as: IP addresses, SNMP community, DHCP server or relly attributes, SSH, ACLs,
routing protocols.

- Ansible playbooks use dynamic inventory, no need to add IP address into inventory file.
- SSH access on Cisco devices is not allowed by default and will be activated with task 
"Run expect commands" with execution of Linux shell commands. 
- run playbook with following arguments: ansible-playbook play_service_one.yml -e service_one_vars -i inventory


.<br>
├── ansible.cfg<br/>
├── collections<br/>
│   └── requirements.yml<br/>
├── CONFIG<br/>
├── group_vars<br/>
│   └── routers.yml<br/>
├── inventory<br/>
├── main<br/>
├── play_service_one.yml<br/>                    
├── play_service_two.yml<br/>
├── play_split_service.yml<br/>
├── README.md<br/>
├── roles                                   # three type of services</br>
│   ├── service_one<br/>
│   │   ├── tasks<br/>
│   │   │   └── main.yml<br/>
│   │   ├── templates<br/>
│   │   │   └── service_one_template.j2<br/>
│   │   └── vars<br/>
│   ├── service_two<br/>
│   │   ├── tasks<br/>
│   │   │   └── main.yml<br/>
│   │   ├── templates<br/>
│   │   │   └── service_two_template.j2<br/>
│   │   └── vars<br/>
│   └── split_service<br/>
│       ├── tasks<br/>
│       │   └── main.yml<br/>
│       ├── templates<br/>
│       │   └── split_service_template.j2<br/>
│       └── vars<br/>
├── service_one_vars                         # include all variable<br/> 
├── service_two_vars<br/>
└── split_service_extravars<br/>
 
