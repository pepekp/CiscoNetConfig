 Cisco IOS, IOS-XE configuration with Ansible
 
.
├── ansible.cfg<br/>
├── ansible.log<br/>
├── collections<br/>
│   └── requirements.yml<br/>
├── CONFIG<br/>
├── group_vars<br/>
│   ├── jumpserver.yml<br/>
│   └── routers.yml<br/>
├── inventory<br/>
├── main<br/>
├── play_service_one.yml<br/>                    
├── play_service_two.yml<br/>
├── play_split_service.yml<br/>
├── README.md<br/>
├── roles                                   # three type of services
│   ├── service_one
│   │   ├── tasks
│   │   │   └── main.yml
│   │   ├── templates
│   │   │   └── service_one_template.j2
│   │   └── vars
│   ├── service_two
│   │   ├── tasks
│   │   │   └── main.yml
│   │   ├── templates
│   │   │   └── service_two_template.j2
│   │   └── vars
│   └── split_service
│       ├── tasks
│       │   └── main.yml
│       ├── templates
│       │   └── split_service_template.j2
│       └── vars
├── service_one_vars                         # include all variable 
├── service_two_vars
└── split_service_extravars
 
