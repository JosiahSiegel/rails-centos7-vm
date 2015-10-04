## Ruby on Rails CentOS 7 Virtual Environment

### Requirements
* [VirtualBox](https://www.virtualbox.org/)
* [Vagrant](http://www.vagrantup.com/)

### Built-in Features
* Leave your ruby version worries behind with [rbenv](https://github.com/sstephenson/rbenv)
* MySQL is ready to go upon VM bootup
* Rails (3000) & MySQL (3306) ports are already open in [firewalld](https://access.redhat.com/documentation/en-US/Red_Hat_Enterprise_Linux/7/html/Security_Guide/sec-Using_Firewalls.html)
* The Vagrantfile is configured to give your host access to the above ports

### Specifications
* Ruby 2.2.2
* Rails 4.1.9
* MySQL 5.6.27

### Installation
```sh
$ git clone https://github.com/JosiahSiegel/rails-centos7-vm.git
$ cd rails-centos7-vm
$ vagrant up
$ vagrant ssh
```

Access shared folder within VM
```
cd /vagrant
```
