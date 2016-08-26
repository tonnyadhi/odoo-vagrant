# odoo-vagrant

Vagrant Setup for Odoo 9 on Ubuntu 16.04

Dependencies
------------

* [VirtualBox](https://www.virtualbox.org/wiki/Downloads)
* [Vagrant](https://www.vagrantup.com)

Setup
-----

1. Download and install Virtual Box

2. Download and install Vagrant

3. Clone this repo

```
git clone http://github.com/kamaxeon/odoo-vagrant.git
```

4. Start virtual machine

```
cd odoo-vagrant
vagrant up
```

5. Login in the virtual machine, and start odoo


```
vagrant ssh
~/odoo-dev/odoo/odoo.py -d v9dev
```

6. Open your browser and go http://localhost:8069 (admin:admin)

Shared folders
--------------
src/my_addons is mapped to /home/vagrant/my_addons, you can write your modules in this directory


Contributing
------------

1. Fork it
1. Create your feature branch (`$ git checkout -b my-new-feature`)
1. Commit your changes (`$ git commit -am 'Add some feature'`)
1. Push to the branch (`$ git push origin my-new-feature`)
1. Create new Pull Request
