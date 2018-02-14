# docker-registry-private-withauth
Run your own docker registry with authentication

Uses https://github.com/mkuchin/docker-registry-web - simple Web UI for Docker Registry
The configuration is taken from https://github.com/mkuchin/docker-registry-web/tree/master/examples with minor updates I needed. See https://github.com/mkuchin/docker-registry-web for more configuration explanations


1. You need docker and docker-compose to be installed on your machine
2. Make sure you have a "big disk" mapped to /data/RegistryData or change docker-compose.yml to use your path to where do you want to map registry data
3. Run ./generate-keys.sh
4. Run
docker-compose up -d

5. Goto http://<yourhost>:5000 for your registry WebUI
Add users, roles, etc
6. Don't forget to configure your docker engine to work with your new registry and then docker login
