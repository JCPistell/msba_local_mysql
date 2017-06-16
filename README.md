## Local mysql server for MSBA students

This vagrantfile spins up and provisions a mysql server with two test databases - good for testing mysql workbench functionality.

### Prerequisites

1. Install [Virtualbox](https://www.virtualbox.org/wiki/VirtualBox)
2. Install [Vagrant](https://www.vagrantup.com/)
3. Install [Git](https://git-scm.com/) if you don't have it already.

Fire up a terminal and navigate to an appropriate parent directory, then clone this repo:

```
git clone https://github.com/JCPistell/msba_local_mysql.git
```

Then vagrant up:

```
cd msba_local_mysql
vagrant up
```

Once the provisioning is done you can access your database with the following settings:

Host: 192.168.56.101
Port: 3306
Username: msba
Password: msba2018

Once you are done testing you can shut down the VM with `vagrant halt` or get rid of it completely with `vagrant destroy`. If you need to bring it up again simply do `vagrant up` and you're good to go!
