## GUIDE TO RUN MONOALG_3D ON A DOCKER CONTAINER

----------------------------------------------------------

This guide provides instructions on how to run MonoAlg3D using [docker](https://www.docker.com/) containers.
Both a CPU-only and a GPU versions are provided.

> [!NOTE]
> You may need to run the following commands with `sudo`.

### CPU only version
1. Build the docker image
```sh
    $ docker build -t monoalg3d:cpu -f Dockerfile.cpu .
```
2. Run the image in interactive mode
```sh
    $ docker run -it monoalg3d:cpu
```

### GPU version
1. Install [Nvidia Container Toolkit](https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/latest/index.html) on your machine following the official instruction.
2. Build the docker image
```sh
    $ docker build -t monoalg3d:gpu -f Dockerfile.cuda .
```
3. Run the image in interactive mode
```sh
    $ docker run -it monoalg3d:gpu
```
