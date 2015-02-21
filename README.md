# Purpose

A base setup for creating a running virtual machine using [Vagrant](https://www.vagrantup.com/) and provisioning [Sonatype Nexus](http://www.sonatype.org/nexus/) on the VM using [Ansible](http://docs.ansible.com/index.html).

# Getting Started

1. [Install VirtualBox]()
2. [Install Vagrant](https://docs.vagrantup.com/v2/installation/index.html)
3. [Install Ansible](http://docs.ansible.com/intro_installation.html#installation) (I recommend [Homebrew](http://brew.sh/) for OS X)
4. Open a terminal
5. ````git clone git@github.com:JGailor/nexus-vagrant-ansible.git````
6. ````cd nexus-vagrant-ansible````
7. ````vagrant up````

You should now have a provisioned VM running Nexus.  It is configured so that your Virtual Machine is accessible at ````192.168.50.4````

To access the Nexus server, point your browser at http://192.168.50.4:8081/nexus/
