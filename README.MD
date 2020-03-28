## Flaskr an example application written in Python/Flask [![Codefresh build status]( https://g.codefresh.io/api/badges/pipeline/pangborn.consulting.llc/CodeFresh%20-%20Training%20Project%2Fbasic-build?key=eyJhbGciOiJIUzI1NiJ9.NWU2Njk0MzJiOTg3M2YzM2Y4NmM4ZTVm.LGBZv091Q3c9j4BssRGRKuU7bwZeFvMcTkP0_PY-VX4&type=cf-2)]( https%3A%2F%2Fg.codefresh.io%2Fpipelines%2Fbasic-build%2Fbuilds%3Ffilter%3Dtrigger%3Abuild~Build%3Bpipeline%3A5e7f5c461fbc96279cb213de~basic-build)

![Flask plus Codefresh](docker-flask-codefresh.jpg)

Original source code from https://github.com/pallets/flask/tree/master/examples/tutorial

## Docker instructions

To create a docker image execute: 

`docker build . -t flaskr`

To run the docker image execute:

`docker run -p 5000:5000 flaskr` and visit with your browser http://localhost:5000

To run unit tests inside the container execute:

`docker run -it flaskr /bin/sh`

and then in the new command promt run

`pip install pytest && pytest`

## To use this project in Codefresh

There is also a [codefresh.yml](codefresh.yml) for easy usage with the [Codefresh](codefresh.io) CI/CD platform.

More details can be found in [Codefresh documentation](https://codefresh.io/docs/docs/getting-started/create-a-basic-pipeline/)
