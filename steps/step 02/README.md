# DockerKeycloakApacheSample
Sample project to setup an environment with Keycloak

This is my personal research project, I <i>may</i> document it later.
# Start the project
## Requirement
Docker Installation
## Start the project
Pull the project to your development machine.
Create Docker Networks from create_network.sh file. Either run it directly (Linux only) or execute the docker commands in the file manually.
Open a shell inside the root folder and start up docker containers with:
``docker-compose up &``

## Test Project
Open ``http://localhost`` in your browser.
You will find a simple page with three links:
*  ``http://localhost/public``
*  ``http://localhost/private``
*  ``http://localhost/auth``

Open ``http://localhost/public`` and you will see the public page.
Open ``http://localhost/private`` and you will see the private page.
Open ``http://localhost/auth`` and you will see the <i>Welcome to Keycloak</i> page.

## Keycloak credentials
This are the Keycloak credentials for the administrative user:
* Username: admin
* Password: admin

# Steps of my project
## Step 01 - Apache HTTPD servers
Setup a docker environment with three Apache HTTPD servers:
* Public Pages
* Private Pages
* Reverse Proxy

## Step 02 - Add Keycloak
Add Keycloak with a PostgreSQL database to the setup.

