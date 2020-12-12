# Generate docker image with ruby-1.9.3p551

Build ruby-1.9.3p551 image

```bash
❯ docker pull encoreshao/ruby-1.9.3p551
```

### Build and test your image

```bash
❯ docker build --rm=true -t ruby-1.9.3p551 .
```

#### View all images

```bash
❯ docker images
REPOSITORY                  TAG                 IMAGE ID            CREATED             SIZE
ruby-1.9.3p551              latest              737fb48e37f8        27 seconds ago      718MB
```

#### Removes all images that match the specified ID 
```bash
❯ docker rmi -f 737fb48e37f8
```

### Use the image to create a new container

```bash
❯ docker run -it ruby-1.9.3p551
```

#### View all containers

```bash
❯ docker container ls
CONTAINER ID        IMAGE               COMMAND             CREATED             STATUS              PORTS               NAMES
b284fd29efc6        ruby-1.9.3p551      "irb"               6 seconds ago       Up 6 seconds                            clever_franklin
```

### Start a container

```bash
> docker start -i 1df18a504ddc
```