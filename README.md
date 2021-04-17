# recoll-docker-compose

## What is this?
This is an repo holding an docker-compose and Dockerfile which will start an container with recall and expose the WebUI for Recoll on port 8080. The files to be indexed can be configured in the docker-compose.yml.

## How to use
1. check the `docker-compose.yml` and modify the to-be-searched dir as you like
2. run `docker-compose up -d` and give the container some time to index
3. open `http://localhost:8080` and start searching you files

## Credits
- many thanks to the creators of recoll and recoll-webui
