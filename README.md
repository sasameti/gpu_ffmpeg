# gpu_ffmpeg
The repo for the gpu enabled Docker Container with FFMPEG specially combined


# Intro:
This docker file extends the _nvidia/cuda_ docker image and builds the ffmpeg on top of it so it can use the GPU.

# How to use?
In order to Run a container Use the following command:

docker container run -it --runtime=nvidia -e NVIDIA_VISIBLE_DEVICES=all -e NVIDIA_DRIVER_CAPABILITIES=compute,utility,video sajad93/gpu_ffmpeg bash

You also replace _bash_ in the command above with any command you need.
