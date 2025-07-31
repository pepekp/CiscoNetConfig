 Cisco IOS, IOS-XE configuration with Ansible
 
.<br>
├── ansible.cfg<br/>
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
 
