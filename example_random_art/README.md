# Example | Generate Random Art

This example is inspired by https://www.freecodecamp.org/news/how-to-create-generative-art-in-less-than-100-lines-of-code-d37f379859f/
Main elements of the code where taken form this blog post. I did some minor modifications to meet python3 standards and added a cli.


# Random Art

Fore more infromations please read, like and share the article of Eric Davidson at [www.freecodecamp.org](https://www.freecodecamp.org/news/how-to-create-generative-art-in-less-than-100-lines-of-code-d37f379859f/) .


## Basic Usage

### Install
1. This project uses poetry for dependency management. First install poetry via pip
`pip install poetry`

2. Run poetry install in this directory
`poetry install`

### Run Script
This script provides a command line interface to specify the parameters of your experiment .
`'sprithering.py -o <output_folder> -g <grid_size> -i <invaders> -s <img_size> -n <samples>'`

<ADD IMAGES HERE>

## Docker Container
The example is packed into a simple python docker container. The container is available in this repositories container registry.

### (Install Docker)
https://docs.docker.com/get-docker/

### Pull Docker container
`docker pull docker.pkg.github.com/michaelwittmann/docker_simulation_pipeline_example/random-art-image:latest`

### Run Docker container
```bash
docker run --name RandomArt -it --mount type=bind,src=C:\Users\gu92jih\docker_sim,dst=/mnt/output/ docker.pkg.github.com/michaelwittmann/docker_simulation_pipeline_example/random-art-image:latest -o /mnt/output -g 15 -i 30 -
s 5000 -n 2
```