# Ethereum Mining with GPU NVIDIA/CUDA-Enabled Docker Container

This is a straightforward docker container using the NVIDIA/CUDA enabled docker container ```nvidia/cuda:11.2.0-devel-ubuntu20.04``` as a base. NVIDIA/CUDA requires the host machine to have updated drivers.

## Running ethminer

```bash
docker run --gpus all --rm -it xychelsea/ethminer:latest ethminer
```

## Building the container

```bash
docker build -t xychelsea/ethminer:latest-gpu -f Dockerfile.nvidia .
```
