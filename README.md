# Docker Postgis Suite

This repo contains a couple of docker, docker-compose and configuration files, that integrated allow to run a postgis "suite" with different tools (ie. pgadmin, backup, cronjobs, etc).

# How to use it

### Start
  - Download repo to local environment
  - If you want to see db-backup in action, change backups-cron file permission and owner as follow:
  ```sh
     $ chmod 644 backups-cron 
     $ chown root:root backups-cron
  ```
    You can edit the backups-cron file and then enable bd backup with a different cron definition (currenlty it will save the backup in pg/dbbackups folder every 1 min)
  - Execute ./start.sh script

### Stop
  - Execute ./shutdown.sh script
  

# Todos

 - Integrate Crontab-ui in kartoza/pg-backup image

License
----

MIT