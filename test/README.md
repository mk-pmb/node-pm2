
# Installing development version

```bash
$ npm install git://github.com/Unitech/pm2.git#development -g
```

# Redhat

```
$ sudo yum install git wget emacs
$ sudo yum groupinstall "Development Tools"
$ wget -qO- https://raw.github.com/creationix/nvm/master/install.sh | sh
$ # put .bash_profile content to .bashrc
$ source .bashrc
$ nvm install v0.11.10
$ nvm alias default 0.11.10
$ npm install pm2 -g
$ # OR
$ npm install git://github.com/Unitech/pm2.git#development -g
```

# CentOS

```
$ yum install git wget emacs
$ wget -qO- https://raw.github.com/creationix/nvm/master/install.sh | sh
$
```

## Remove init script

```
$ chkconfig --del pm2-init.sh
$ chkconfig --add pm2-init.sh
```

gyp WARN EACCES user "root" does not have permission to create dev dir :
https://github.com/TooTallNate/node-gyp/issues/126
-> add --unsafe-perm
