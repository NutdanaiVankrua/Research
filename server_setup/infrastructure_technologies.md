## Server side technologies/infrastructure

### Servers

* [NGINX](https://www.nginx.com/): Web server, distribution static file & proxy
* [Unicorn](https://bogomips.org/unicorn/): Rack server, web server for rails
* [Supervisord](http://supervisord.org/): Monitoring process and auto restart if dead process, nginx, unicorn, mysql, redis, etc.
* [Redis](https://redis.io/): Cache, store user, session data
* [Mysql](https://www.mysql.com/): Database
* [Bundler](http://bundler.io/): Manage library of Ruby, gemfile
* [Fluentd](http://www.fluentd.org/): log collector. save log and upload to s3
* [ngx_small_light](https://github.com/cubicdaiya/ngx_small_light): A dynamic image transformation module for nginx.

### Setup Machine
* [Vagrant](https://www.vagrantup.com/): wrapper for virtualbox. Create and configure lightweight, reproducible, and portable development environment.
* [Docker](https://www.docker.com/): software containerization platform
* [Ansible](): operate setup task via ssh. setup local vm, staging, production setup by this
* [Capistrano](http://capistranorb.com/): deploy source code