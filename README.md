Pushy
=====
A push notification service for Google Calendar

Description
-----------
To my knowledge, Google's Calendar API doesn't offer good push notification abilities. So if you want them to push new events to your server, you're out of luck. This is a simple service that allows users to connect to Google Calendar via OAUTH2. The service then has a script that can be run as a cronjob periodically, which checks to see if there are any new events to pull down and notify

Installation
------------
This application is written in PHP, including the cron script. To set up this application, put its code on an Apache webserver (or other server of your choice). There is an included SQL script in the sql directory, which you should pipe into your mysql command in order to set up the mysql database. The cron script is located in the "cron" directory, and you can set that to run in your /etc/crontab file
