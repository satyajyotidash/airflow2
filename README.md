# Airflow2 with MSSQL 
Airflow2 with mssql. This installs with pre defined airflow2.tar.gz file. if you have an existing setup , please make tar.gz file from airflow home where airflow.cfg and webserver_config.py files exists.This Also should exist python virtual environment with python version 3.6.
1. Role name is airflow2 
2. Tasks prereqs ,setup (setting the enviroment for airflow installation) , install and services 
3. Called by airflow2.yml from base directory with role airflow2
4. This Creates admin user 'airflow' for WebUI loggin -> pass is in vars file , also if your using ldap authuntications , it will work as expected 
5. It stops firewalld service and starts webserver services only as you need to start services manully as per its(instance) role 

Note: 1.Please make sure you have updated airflow.cfg (from files) and webserver_config.py.
      2.Make sure you opned all required ports are opened like 1433 for mssql ,8080 for webui..etc to all services part of airflow2 instance 



