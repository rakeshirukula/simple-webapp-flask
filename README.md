# Simple Web Application

This is a simple web application using [Python Flask](http://flask.pocoo.org/) and [MySQL](https://www.mysql.com/) database. 
This is used in the demonstration of development of Ansible Playbooks.
  
  Below are the steps required to get this working on a base linux system.
  
  - Install all required dependencies
  - Install and Configure Web Server
  - Start Web Server
   
## 1. Install all required dependencies
  
  Python and its dependencies

    apt-get install -y python python-setuptools python-dev build-essential python-pip python-mysqldb

   
## 2. Install and Configure Web Server

Install Python Flask dependency
Install pip packages according to python version lastest is python3
   

    pip3 install flask
    pip3 install flask-mysql

- Copy app.py or download it from source repository
- Configure database credentials and parameters 
- COPY THE CODE FROM APP.PY & PASTE IN ANY DIRECTORY EX: /HOME/app.py
## 3. Start Web Server

Start web server

    FLASK_APP=/home/app.py flask run --host=0.0.0.0
    
## 4. Test

Open a browser and go to URL

    http://<IP>:5000                            => Welcome
    http://<IP>:5000/how%20are%20you            => I am good, how about you?
