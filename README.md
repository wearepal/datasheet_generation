## Causal datasheet REPO. 

This repo is for generating statistics used in the datasheets found in the 'Causal Datasheet' paper.

To run the code first install the python requirements from the requirements.txt:

`pip install -r requirements.txt`

Following this, R, and some R libraries must be installed:

`apt-get -q install r-base -y --allow-unauthenticated`
`Rscript -e 'source("http://bioconductor.org/biocLite.R"); biocLite(c("CAM", "SID", "bnlearn", "pcalg", "kpcalg", "D2C"))'`

Finally, one can then open the jupyter notebook with:

`jupyter notebook`