# mysql-cleaner
Very simple bash script that will help you kill any MySQL connections that have been sleeping longer than defined 'n' amount of time.

# Setup
`$ chmod +x mysql-cleaner`

you may add these in your path variable via your **~/.bash_profile** file

Modify the MAX_SLEEP_TIME variable in mysql-cleaner in case you would like to kill the sleeping processes quicker default is 60 seconds

Also add MYSQL_USER and MYSQL_PASS in same file

## Usage of mysql-cleaner
You can also run it as a cron job, the cron would look something like this:

`*/2 * * * * /path/to/the/script/mysql-cleaner /dev/null 2>&1`

above will check in every 2 mins. and kill slept mysql queries/process
