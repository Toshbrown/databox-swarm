
# Uasge 

    npm install 
    ./getCompnentSrc.sh
    ./startDatabox //Take a while first time as it builds all the needed images

# why refactor 

move to docker swarm - better secrets management, ability (in future) to run databox across may devices, makes moving to linuxkit possible 

Build the whole platform using docker-compose build

Seems more stable and decreased startup time  

Removes the need for the local registry mirror in dev mode


# Left to fix 

The cm ui is looking for containers not services 

The cm ui should be split out from the CM api (security ui's dint need access to the docker socket, and flexibility)

Export service update certs and keys 

Removing keys on shutdown

Fix order of launching platform containers

ARM support