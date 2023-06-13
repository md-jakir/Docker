# DOCKER

# Docker import and export:

Note: docker will export for only the stopped container not for running container

$ docker export [container_ID or container_name] >/path/to/container_name.tar

Note: Export file can be different based on image like when export nginx stopped container by default, it won't have the default command. That's why when import image from exported tar file and run container it will prompt for a command to run. 

$ docker run -d -p 8080:80 myapp:v1 nginx -g 'daemon off;'


