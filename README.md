# GoCD server inside of Docker container

Install:

``git clone https://github.com/codesshaman/docker_gocd_server.git``

Build:

``make build``

or

``docker-compose up -d --build``

Connect:

``http://your_host:8153``

Down:

``make down``

or

``docker-compose down``

Up:

``make``

or

``docker-compose up -d``

If neceary, uncommit volumes lines for acess to gocd configs in the filesystem, or use command:

``docker exec -it gocdserver cat /godata/config/cruise-config.xml | grep agentAutoRegisterKey=``

for show agent autirised key.
