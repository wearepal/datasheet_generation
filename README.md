## Causal datasheet REPO. 

This repo is for generating statistics used in the datasheets found in the 'Causal Datasheet' paper.

These experiments are dependent on the structure learning algorithms found in the Causal Discovery Toolbox Python library (https://fentechsolutions.github.io/CausalDiscoveryToolbox/html/index.html). As well as it's own implementations, this library wraps around many useful R libraries. Installing these correctly can be a difficult process, and so we have pre-installed all the required libraries into a docker image.

To run the code first install docker: https://docs.docker.com/get-docker/

Then, pull the docker image for this repository:

`docker pull braddpbutcher/causal_datasheet`

Launch the docker container with:

`docker run -it -p 8888:8888 braddpbutcher/causal_datasheet /bin/bash`

Navigate into the Causal Datasheet repo folder:

`cd causal_datasheet`

Finally, run the notebook with:

`jupyter notebook --ip 0.0.0.0 --no-browser --allow-root`