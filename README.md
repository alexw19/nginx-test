## INSTRUCTIONS FOR RUNNING SCRIPT

* Rename run.sh.test in proxy/ to run.sh and chmod +x 
* Run commands below
```
cd proxy/
docker build --tag nginx-test:0.0.1 .
cd ../web
docker build -t webserver-image:v1 .
cd ..
docker-compose up
```
