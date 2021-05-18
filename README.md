# ncov-humboldt

This repo describes how to conduct the phylogenetic analysis described in the manuscript. You will also find figures and additional scripts that we used for parsing data and making figures.

## Phylogenetic inference using nextstrain
To reproduce this analysis you'll need to have Nextstrain installed. Documentation on installing Nextstrain is available [here](https://docs.nextstrain.org/en/latest/install-nextstrain.html).

This analysis also makes use of the Nextstrain team's `ncov` analysis repo, which you can find [here](https://github.com/nextstrain/ncov). We recommend cloning this repo to your local machine and running the analysis within that repo (this will ensure all software components are up-to-date with the Nexstrain team's ncov builds).

### To run the analysis

The Nextstrain `ncov` builds use "profiles". You'll see in this repo that there is a directory called `my_profiles`, and within that directory there is another directory called `humboldt`. You'll want to move the `humboldt` directory over the the `my_profiles` directory within the `nextstrain/ncov` repo.

Once you have conda installed you can create the environment by running

`conda env create -f humboldt-analysis-env.yaml` within the top level directory of this repo.

Then, to load the environment run

`conda activate humboldt-analysis`

To open the jupyter notebooks you can run

`jupyter notebook analysis-scripts/<notebook_name>` within the top level directory of this repo.

## Additional analysis

To run the additional scripts in `analysis-scripts` you'll want to create a new conda environment from our environment file. If you do not already have conda installed you can find install directions [here](https://conda.io/projects/conda/en/latest/user-guide/install/index.html).
