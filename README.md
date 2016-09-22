# ubuntu-trusty-drupal-2

docker build -t ubuntu-drupal https://github.com/ningappa/ubuntu-trusty-drupal-2.git

docker run -d --name 6thstreet -v /6thstreet -e MYSQL_PASS=6thstreet -e VIRTUAL_HOST=www.6thstreet.xyz  -e VIRTUAL_DOMAIN=www.6thstreet.xyz -e MYSQL_USER=mydbuser -e MYSQL_PASS=mydbpassword -e MYSQL_DBNAME=mydbname -e WP_USER=admin123 -e WP_PASS=pass1233 -e USER_EMAIL=ningappa@poweruphosting.com  ubuntu-drupal
