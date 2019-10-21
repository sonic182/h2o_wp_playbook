
# Requirements

* Python 2 or 3
* ansible
* virtualbox (optional, for testing)
* vagrant (optional, for testing)

# This does

* Copy local wordpress (obtained by executing `bash get_wp.sh`)
* Install [h2o](https://h2o.examp1e.net/) provided by OS 
* Install Php7.X and dependencies
* Install mariadb 10
* Install memcached
* Install certbot
* Configure folders permissions
* Configure mariadb users
* Configure h2o Fastcgi
* Starts h2o
* Restarts h2o (In case you execute `vagrant provision` to re-execute ansible in vagrant guest)


# Python 2/3

Actually by the `local_python` variable in the `playbook` you can specify the python version you're using for ansible in your local (host) machine, by specifying `python` or `python3`

# Letsencrypt

You have to manually access to your remote machine and configure the new certificate.
