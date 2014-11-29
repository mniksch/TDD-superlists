## Required packages:

* Python 3.4
* Django 1.7
* Git
* pip
* virtualenv

##site setup:

export SITENAME=site.collegebot.org
mkdir -p ~/$SITENAME/database
mkdir -p ~/$SITENAME/public/static
mkdir -p ~/$SITENAME/virtualenv
git clone (https://github.com/mniksch/TDD-superlists.git ~/$SITENAME/source

##then copy the virtualenv from a different folder and change path
##in the bin/activate script (to the new SITENAME path)

#Then copy the passenger_wsgi.py (from TEMPLATE) into $SITENAME and
#change 'modulename' to the name of the Django module

#manage.py migrate for database

#collectstatic for static files

#Set DEBUG=False and ALLOWED_HOSTS in settings.py

#Run FTs to check everything works

## Folder structure:
Assume user account /user/mniksch
/user/mniksch
|--sitename
   |--database
   |--source
   |--public
      |-static
   |--virtualenv
