# netFortune
[![Build Status](https://travis-ci.org/ArtemAlagizov/net-fortune.svg?branch=master)](https://travis-ci.org/ArtemAlagizov/net-fortune)


A learning project to develop a networked "fortune" clone in Haskell.

Github repository of the app: 
````
https://github.com/ArtemAlagizov/net-fortune
````
Docker container with the app: 
````
https://hub.docker.com/r/alagiz/net-fortune/
````

# Usage with docker
* Run
```
$ docker pull alagiz/net-fortune
```
```
$ docker run -i -t -p 8080:8080 alagiz/net-fortune /bin/bash
```
* Visit http://localhost:8080/fortune or http://host-ip:8080/fortune (default is http://192.168.99.100:8080/fortune)
  * To get docker host ip run
    ```
    $ docker-machine env
    ```  

# Usage without docker

* Have stack installed
    ```
    https://docs.haskellstack.org/en/stable/README/
    ```
* Run 
    ```
    $ stack build
    ```
    ```
    $ stack exec netFortune-exe
    ```
* Visit http://localhost:8080/fortune
