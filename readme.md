<div align="center">

# Docker image for Audiocraft

[![python](https://img.shields.io/badge/python-3.10-green)](https://www.python.org/downloads/)
[![cuda](https://img.shields.io/badge/cuda-12.4-green)](https://developer.nvidia.com/cuda-downloads)

<p align="center">
  <img src="assets/banner.PNG" />
</p>
</div>

## Tags
| Tag    | Description              | Size      |
| ------ | ------------------------ | --------- |
| latest | python 3.10, audiocraft 2.0.1 | ~ 7.7 GB |

## Ports

| Connect Port | Internal Port | Description |
| ------------ | ------------- | ----------- |
| 7860         | 7860          | Audiocraft  |
| 8888         | 8888          | Jupyter Lab  |

## Running locally
```bash
docker run -d \
  --gpus all \
  -p 7860:7860 \
  -p 8888:8888 \
  yuvraj108c/audiocraft-plus:latest
```

## Building the docker image
```bash
git clone https://github.com/yuvraj108c/audiocraft-plus-docker
cd audiocraft-plus-docker

docker-compose build latest
```

## Credits
https://github.com/GrandaddyShmax/audiocraft_plus/

## License
CC BY-NC-SA 4.0