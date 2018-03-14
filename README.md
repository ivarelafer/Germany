# Germany
A simple Docker, Vagrant, and Ansible automation task.

This project is based on a Vagrant file that launch a Centos7 minimal Virtual machine running on VirtualBox. The vagrant file calls Ansible to automate the provisioning of the VM.

Ansible playbook installs and runs Docker in Centos7 VM, pull an Alpine Docker Linux image, build a new Docker custom Alpine Linux with an nginx web server configured to serve HTTP and HTTPs requests.


You can store the sites data to this directory structure:

```
/www
├─── website1_files
|    └ ...
└─── website2_files
     └ ...
/etc
└─── nginx
	 └─── conf.d
	 	  ├─── website1.conf
	 	  └─── website2.conf
```
