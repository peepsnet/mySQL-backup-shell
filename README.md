# mySQL-backup-shell
from: https://www.matteomattei.com/how-to-backup-mysql-database-using-shell-and-cron/

chown root.root backup.sh
chmod 770 backup.sh

Then, to set a cronjob to do it automatically every day, open /etc/crontab and add the following line at the bottom:

# mysql backup
32 4  *  *  *   root    /root/mysql_backup.sh
