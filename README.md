# GoCD server inside of Docker container

Install:

``git clone https://github.com/codesshaman/docker_gocd_server.git``

Create volume folder:

``mkdir ~/.gocd``

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

Howto check agent registery key on container:

``docker exec -it go-server cat /godata/config/cruise-config.xml | grep "agentAutoRegisterKey="``

Howto check agent registery key on filesystem:

``cat ~/.gocd/cruise-config.xml | grep "agentAutoRegisterKey="``