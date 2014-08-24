<h2>Vagrant and Puppet configuration for NodeJS, Redis, MongoDB, & Meteor</h2>

Vagrant configuration with puppet to create a Virtual Box machine with 
Ubuntu Server x64 14.04, Nodejs v0.10.\*, Redis stable release, MongoDB 
2.6.\*, and the latest Meteor release.


Installation:<br>
Install Vagrant 1.6.x<br>
Install Virtual Box 4.3.12<br>
Clone the repository <strong>git clone https://github.com/artribou/vagrant-nodejs-redis-mongodb-meteor.git</strong><br>

* CD - cd vagrant-nodejs-redis-mongodb-meteor
* Run - vagrant up<br>
* SSH - vagrant ssh<br>
* Halt - vagrant halt<br>


access mongo and redis from your machine:

* redis.cli h 192.168.33.10 -p 6379<br>
* mongo 192.168.33.10


use meteor:

* vagrant ssh
* cd /home/vagrant/meteor
* meteor create myapp
* mkdir ../myapp-local
* ln -s ../myapp-local myapp/.meteor/local
* cd myapp
* meteor


Puppet Manifest will install:
[Nodejs - v0.10.\*, Redis - last stable release, MongoDB - 2.6.\*, Meteor - last release, wget, git, vim, htop, g++]



Good hacking!!!!!!!!
