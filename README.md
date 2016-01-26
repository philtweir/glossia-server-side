Go-Smart Simulation Architecture (GSSA)
=======================================

**Primary authors** : [NUMA Engineering Services Ltd](http://www.numa.ie) (NUMA), Dundalk, Ireland

**Project website** : http://www.gosmart-project.eu/

This project is co-funded by: European Commission under grant agreement no. 600641.

This set of containers and scripts provides a means for setting up a GSSA server using docker-compose.
Please note that the provided docker-compose.yml will start a Crossbar instance also - if you wish to
connect to an existing Crossbar instance, use `docker run` with arguments based on those in the
docker-compose.yml file.

Usage
-----

The simulation server (GSSA) may be launched by the command

```sh
    cd compose
    sudo docker-compose up -d
```

Note that the host must have a running `dockerlaunchd` instance, with a socket in
`/var/run/docker-launch/docker-launch.sock` accessible to the `dockerlaunch`
user group.
