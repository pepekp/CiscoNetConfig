 Cisco IOS, IOS-XE configuration with Ansible
 
.
├── ansible.cfg
├── ansible.log
├── collections
│   └── requirements.yml
├── CONFIG
├── group_vars
│   ├── jumpserver.yml
│   └── routers.yml
├── inventory
├── main
├── play_service_one.yml                    
├── play_service_two.yml
├── play_split_service.yml
├── README.md
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
 
