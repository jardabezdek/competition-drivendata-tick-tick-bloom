## :rocket: competition-drivendata-tick-tick-bloom

Repository with files created for the
[Tick Tick Bloom](https://www.drivendata.org/competitions/143/tick-tick-bloom/)
challenge, organised by [DrivenData](https://www.drivendata.org/).

## :pencil: Authors

- [Jaroslav Bezdek](https://www.github.com/jardabezdek)

## :construction_worker_man: Setup

### Local development

> I wasn't able to install all the requirements within docker image, so I used
virtualenv.

#### Docker

In order to create a working environment, the [docker](https://www.docker.com/)
is used. To start it, please, follow the next steps.

1. Launch the docker daemon.
1. Get to the repository root folder: `cd ~/projects/competition-drivendata-tick-tick-bloom/`
1. Build the docker image with a proper tag: `docker build -t competition-drivendata-tick-tick-bloom:latest .`
1. Run docker container: `docker run -it -p 8888:8888 -v $(pwd):/usr/src/app competition-drivendata-tick-tick-bloom:latest /bin/bash`
1. Run notebook inside the docker container: `jupyter notebook --ip 0.0.0.0 --no-browser --allow-root`

#### virtualenv

1. Create a new virtual environment: `virtualenv --python=python3.8 venv`
1. Activate the virtual environment: `./venv/bin/activate`
1. Install all requirements: `pip install -r requirements.txt`

### Data download

Everything you need is described on the competition page, in the
[Problem description](https://www.drivendata.org/competitions/143/tick-tick-bloom/page/650/)
section.
