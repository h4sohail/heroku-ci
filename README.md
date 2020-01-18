# Heroku CI (Work-in-progress)
Simple Continuous Integration (CI) pipeline for a Python application hosted on Heroku

How it works:

Tracks a github repository for changes, if a change is detected, pulls the source from github and adds Heroku remote url (must be logged into to Heroku cli) then pulls required files from Heroku and updates the Heroku application. Checks every 5 seconds for changes.

How to use:

1. Install Heroku CLI and login to your account.
2. Clone your GitHub repository inside the 'projects' folder.
3. Edit server.py and add your github credentials and other information such as application name.
4. Make the script executable (chmod +x) and run it.
5. Enjoy automatic code deployment to Heroku.
