# WOWMeter
WOWMeter is a click-my-signature website based off the Doge meme. It was started in 2014 by Erman Sayin abandoned a year later, picked up again by Preston Cammarata, closed after a few months, and finally back for good, with a brand new backend.

# Setting up
wow.php is the configuration file that is included in every page, unless the header.php file is doing it for you.

Fill out a random string for the "$salt" variable in wow.php, make it something long, random and unique. This improves security, but make sure to never change it, or all hashed content will be forever lost.

More configuration is self explanatory in wow.php.

Create a database, run the file "db.sql" from the repo in the database in order to get the required tables, make sure you fill out database information in wow.php.

# Notes
When including main.php, type "$no_script = 1" beforehand, to make it not show any content besides the news.

When including the header, type "$login_required = 1" if you want a certain page to be only accessed by logged in members.

When you need to check if the user is logged in, use the boolean "$member_access" to find out.

An array of the logged in users table information is accessed through a variable called "$session_array".

There is a variable that returns the users username. This variable is "$username".

# Extra Scripts
WOWMeter also has server scripts for a few Linux distros that can enable you to update the site from a repo, use cron jobs to find bots, and other stuff, and more. These scripts are not available yet, but will be soon in the repo.

# License
View the LICENSE file for that!