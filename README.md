# django-calendar for COMP-41110
The objective of this excersise was to develop an online calendar that is cloud deployed. 
I followed the 2 tutorials below to build the calendar. 
I modified the calendar so that the static assets (css and image files) are retrieved from AWS S3
and the data is written to AWS RDS. 
I deployed this app on to EC2. Here is the address.
 
ec2-34-240-45-98.eu-west-1.compute.amazonaws.com:8000/calendar

Tutorial for the calendar build part i [here](https://www.huiwenteo.com/normal/2018/07/24/django-calendar.html) and part ii [here](https://www.huiwenteo.com/normal/2018/07/29/django-calendar-ii.html)! :)

# Usage
This is the setup on the ubuntu EC2 server

```bash
    1  git clone https://github.com/duggann3/awsome_calendar.git
    2  sudo apt-get install python3-pip
    3  pip3 install django
    4  pip3 install storages
    5  pip3 install django-storages
    6  pip3 install boto3
    7  sudo apt-get install mysql-server
    8  sudo apt-get install mysql-client
    9  sudo apt-get install libmysqlclient-dev
   10  pip3 install mysqlclient
   11  cd awsome_calendar/
   12  python3 manage.py migrate
   13  python3 manage.py runserver 0.0.0.0:8000
```
