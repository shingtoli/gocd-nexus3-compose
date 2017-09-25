# Compose for GoCD Server & Agent + Nexus3 Repository Manager #

## Description ##
Docker Compose for setting up quickly GoCD server + single NodeJS capable agent and a Nexus3 Repository Manager for development and educational purposes. Dockerfile for GoCD + NodeJS agent is provided.

## Instructions ##

### Nexus3 Repository Manager ###

Run the following within the project directory:

```
docker-compose up
```


Go to http://0.0.0.0:5000 to access Nexus3, setup a npm (hosted) repository and login into the default admin account using:

```
username: admin
password: admin123
email:    admin@example.og
```
On Nexus3, go to settings -> Realms and add `npm Bearer Token Realm` to Active.

### Setting up GoCD ###

Access GoCD with http://0.0.0.0:8153

You may add to the environment variable 'NPM_CONFIG_REGISTRY' to the agent environments.

Enable the agents from Agents and setup your pipelines.
