# Ansible


Web-server ansible_host=172.31.91.26
target2 ansible_host=172.31.94.231
DB ansible_host=172.31.6.214

[webserver]
Web-server
target2

[db]
DB

[dc:children]
webserver
db


 ansible -i inventory -m ping '*'

ansible -i inventory -m ping Web-server
