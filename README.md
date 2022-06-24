# SAE24

SQL On WINDWOS

CREATE USER 'toto'@'%' IDENTIFIED BY 'toto';

FLUSH PRIVILEGES;

GRANT ALL PRIVILEGES ON *.* TO 'toto'@'%'
->     WITH GRANT OPTION;

USE datamining;

SELECT * FROM sensors_data;

to use the data_base.


CMD IN THE VIRTUAL MACHINE

su -

apt-get update

apt-get apache2

service apache2 start

service apache2 status

apt-get install python3 pip apache2 libapache2-mod-wsgi-py3

apt-get install default-mysql-server

apt-get install default-mysql-client

apt-get install default-libmysqlclient-dev

sudo pip3 install virtualenv
    
    <Directory /home/administrateur/django-app/modele>

        <Files wsgi.py>

            Require all granted

        </Files>

    </Directory>


    WSGIDaemonProcess django-app python-home=/home/administrateur/django-app/django-appenv python-path=/home/administrateur/django-app

    WSGIProcessGroup django-app

    WSGIScriptAlias / /home/administrateur/django-app/modele/wsgi.py
