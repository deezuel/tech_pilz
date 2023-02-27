# tech_pilz Task


Docker is a technology that is often used within the DevOps area, and Docker Compose is a useful tool to allow the running on many different docker containers locally as a single solution.

Please create a docker compose configuration which will run 'AT LEAST' the following containers.

Prometheus
Alertmanager
NGINX
A frontend should be available for each of these services on the localhost.

Configure the above system in such a way so as when the NGINX container is down, this is registered in the Prometheus system, which will then send an alert to Alertmanager. This alert should be displayed on the Alertmanager UI. You do not need to configure any routes from the Alertmanager to any other systems such as email or slack.

You may configure the system in any way you like, you can use additional containers if required

# Running
To bring up test environment run:
docker-compose --env-file=compose.env up -d 

Ports configured for containers to be reached at:
Prometheus - http://localhost:9090/targets
Alertmanager - http://localhost:9093/#/alerts
NGINX - http://localhost:8080/
