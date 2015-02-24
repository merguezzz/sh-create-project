# sh-create-project
Bash script using zenity to create project in specific dev environnement to avoid boring job.
- create copy of local default dev repository
- chown/chmod it with $USER:www-data/0775 (Apache2 Daemon)
- create symlink in /var/www
- Add URL line to /etc/hosts
- Create copy of default vhost
- Enable it in Apache2 (and restart)

# TODO
- Handle errors properly and globally
- Option : use DNS method or mod_userdir instead of /etc/hosts
- Make it more generic : config to be used for many dev environnements
- Check if URL is responding correctly at the end
