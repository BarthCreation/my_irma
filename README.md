# my_irma
This is an updated and functionning version of IRMA by Quarkslab

## [How-to] Make IRMA work

My setup: A virtualized Debian 11  
Official IRMA's documentation: [irma.readthedocs](https://irma.readthedocs.io/en/latest/install/index.html)  

###1. Install Vagrant
```console
$ wget -O- https://apt.releases.hashicorp.com/gpg | sudo gpg --dearmor -o /usr/share/keyrings/hashicorp-archive-keyring.gpg
$ echo "deb [signed-by=/usr/share/keyrings/hashicorp-archive-keyring.gpg] https://apt.releases.hashicorp.com $(lsb_release -cs) main" | sudo tee /etc/apt/sources.list.d/hashicorp.list
$ sudo apt update && sudo apt install vagrant
$ vagrant --version
```

###2. Install Ansible
```console
$ sudo apt-get update
$ sudo apt-get install python3-pip
$ sudo pip install ansible
$ ansible --version
```

###3. Install Virtualbox
Process from: [linuxiac.com](https://linuxiac.com/how-to-install-virtualbox-on-debian-11-bullseye/)
```console
$ wget -O- -q https://www.virtualbox.org/download/oracle_vbox_2016.asc | sudo gpg --dearmour -o /usr/share/keyrings/oracle_vbox_2016.gpg
$ echo "deb [arch=amd64 signed-by=/usr/share/keyrings/oracle_vbox_2016.gpg] http://download.virtualbox.org/virtualbox/debian bullseye contrib" | sudo tee /etc/apt/sources.list.d/virtualbox.list
$ sudo apt update
$ sudo apt install virtualbox-7.0
```

