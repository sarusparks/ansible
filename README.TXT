Ansible can connect to any system externally and can perform the task given by us ....
Here we call the ansible modules, every module syntax we can check in the documentation
Module name is mandatory, you can supply argiments to module .. they may be optional or mandatory

ping module

what is ansible playbook
It is list of plays which contain modules that can do specific task.

Inventory
-----------------------
1 or many

inventory.ini --> a file contains a list of servres which ansible connecting to ..

192.168.1.1


variables
datatypes
conditions
fuctions
loops

inheritance --> 

vars_promt

ansible inventory
------------------------
ungrouped
grouped
group of groups

ansible -i inventory.ini ungrouped --list-hosts

data types
-----------------------
string
int, float, double, decimal, long, etc --> number
boolean --> true/false
list
map

ansible is developed using python language 

hosts: web --> target group under web group

{ --> map
[ --> list


conditions
--------------------------
write a playbook to check if number is less than 10 or not

when 
to decide whether the task/module is run or not

create expense user
-----------------
check the expense user already exist or not
if dont exist dont create ot not exist create It

ansible dont have gurantee module exists for everything...
we can use direct commands if module not exists

ansible.builtin.command:

error handling --> handle the errors

if error comes --> ignore errors

facts == variables

ansible, before connections to the servers/hosts it will collect entire information so that it 
can take decisions based on that information.

install nginx
--------------------------
ansible.builtin.dnf
ansible.builtin.apt

loops
-----------------
item --> reserved keyword

fuctions/filters

filter --> manipulation

ansible.builtin.shell
ansible.built.command

command vs shell
--------------------------------
interview question

command --> simple command......... it will not get the shell environtment
shell --> complex pipes, redirections etc... it get the shell environtment

command is secure than shell

expense project
------------------
3 servers, 3records
mysql.daws81.online --> private ip
backend.daws81.online --> private ip
frontend.daws81.online --> private ip
daws81.online --> public ip

ansible is not only configuration management tool , it can also connect to any system if the module is existed


ansible --> aws





