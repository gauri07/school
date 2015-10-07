# school

Welcome All. Please go through this important file to setup your locals.

# Setup only for Linux users

1) sudo apt-get update

2) sudo apt-get install python-pip

3) sudo apt-get install python-virtualenv

4) virtualenv sch

5) . sch/bin/activate

6) pip install django

7) deactivate

8) sudo apt-get install libpq-dev python-dev

9) sudo apt-get install postgresql postgresql-contrib

10) sudo apt-get install nginx

11) . sch/bin/activate

12) pip install gunicorn

13) deactivate

14) sudo su - postgres

15) createdb sch123

16) createuser sch123

17) psql

18) GRANT ALL PRIVILEGES ON DATABASE sch123 TO sch123;

19) \list or \l and scroll down to see whether sch123 db is created with user sch123

20) open new terminal

21) . sch/bin/activate

22) mkdir school

23) cd school

24) git clone https://github.com/shriyanka-kajal/school.git

25) pip install pip install psycopg2

26) edit settings.py file to suit your chosen username and password (may be not required if followed steps)

27) python manage.py syncdb

28) python manage.py migrate

# To fetch from upstream

1) . sch/bin/activate

2) cd school/school

3) git checkout [your branch name]

4) git remote add upstream https://github.com/shriyanka-kajal/school.git (required only once)

5) git fetch upstream

6) git merge upstream/development

# To push to upstream

1) git checkout [your branch name]

2) git status

3) git add [changed file one by one]

4) git commit -m "commit summary"

5) git push origin [your branch name]

# Repositories

`master` actuall product deployment repo. Not to be touched

`development` consists of latest code that is required to be fetched each time while working from your repo

`your repo` your working repo where you will work individually and commit changes from

