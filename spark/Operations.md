`docker build . -t sparkhome`
`docker image ls`
`docker run -p 8888:8888 --name spark -d sparkhome`

Running PySpark from the container
Go to the terminal and go inside the container

`docker exec -it spark /bin/sh`