## Causal datasheet REPO. 

This repo is for generating statistics used in the datasheets found in the 'Causal Datasheet' paper.

These experiments are dependent on the structure learning algorithms found in the Causal Discovery Toolbox (CDT) Python library (https://fentechsolutions.github.io/CausalDiscoveryToolbox/html/index.html). As well as it's own implementations, this library wraps around many useful R libraries. Installing these correctly can be a difficult process, and so we have pre-installed all the required libraries into a docker image.

### Installation via Docker

To run the code first install docker: https://docs.docker.com/get-docker/

Then, pull the docker image for this repository:

`docker pull braddpbutcher/causal_datasheet`

Launch the docker container with:

`docker run -it -p 8888:8888 braddpbutcher/causal_datasheet /bin/bash`

Navigate into the Causal Datasheet repo folder:

`cd datasheet_generation`

Run the notebook with:

`jupyter notebook --ip 0.0.0.0 --no-browser --allow-root`

Finally, navigate to:

`http://127.0.0.1:8888/tree`

accessed using the token provided in the terminal.

### Alternative Installation

If you would like to avoid using docker, you will need to install the Python libraries found in the `requirements.txt` file.
Additionally, as mentioned above, the CDT library requires additional R libraries to function.
Namely:

- R > 3.6 
- BNLearn
- PCALG
- RCIT
- kpcalg
- SID
- CAM
- V8
- clue
- randomForest
- lattice
- devtools
- MASS
- momentchi2
- devtools
- sparsebn

Docker installation is reccomended.
