# DE_Assignment2
To run this application for Jordan dag, follow the next steps:
1- make these directories 
 mkdir ./dags ./logs ./plugins ./data ./output
2- echo -e "AIRFLOW_UID=$(id -u)\nAIRFLOW_GID=0" > .env
3- init the airflow 
 docker-compose up airflow-init
4- get the docker compose up
 docker-compose up -d
5- now you can find the png in output file and the CAVs in the data file 
6- open pdamin and connect to the server 
docker ps 
docker inspect <container id>
new server >> gateway: 172.22.0.1 
           >> username: airflow
           >> password: airflow
7- docker-compose down 