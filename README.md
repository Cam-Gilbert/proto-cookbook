# Prototype Cookbook

<img src="thumbnails/thumbnail.png" alt="thumbnail" width="300"/>

[![nightly-build](https://github.com/ProjectPythia/cookbook-template/actions/workflows/nightly-build.yaml/badge.svg)](https://github.com/ProjectPythia/cookbook-template/actions/workflows/nightly-build.yaml)
[![Binder](https://binder.projectpythia.org/badge_logo.svg)](https://binder.projectpythia.org/v2/gh/ProjectPythia/cookbook-template/main?labpath=notebooks)
[![DOI](https://zenodo.org/badge/475509405.svg)](https://zenodo.org/badge/latestdoi/475509405)

_See the [Cookbook Contributor's Guide](https://projectpythia.org/cookbook-guide) for step-by-step instructions on how to create your new Cookbook and get it hosted on the [Pythia Cookbook Gallery](https://cookbooks.projectpythia.org)!_

This Project Pythia Cookbook covers using ERA5 reanalysis data to explore potential flood events in Alabama and compare them to data collected by my teammates who have paleo soil cores for the time period that we can investigate.

## Motivation

This cookbook will be useful to explore portions of the ERA5 reanalysis dataset, as well as explore connections between events shown in the reanalysis and flood events seen in soil core samples. For this homework I have just simply gone through the process of identifying a single event, and plotting that event using geoviews animations. 

## Authors

[Cameron Gilbert](https://github.com/Cam-Gilbert), etc. _Acknowledge primary content authors here_

### Contributors

<a href="https://github.com/ProjectPythia/cookbook-template/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=ProjectPythia/cookbook-template" />
</a>

## Structure

Notebook 1 - Describes the process of identifying events

Notebook 2 - Describes the process of making an animation of 3 days of precipitation 

### Identifying precipitation events

Contained in Notebook 1. Describes the process of identifying events using the hourly precipitation variable.

### Animating precipitation events

Contained in Notebook 2. Describes the process of creating a simple animation of the hourly precipitation variable through time. Creates a radar like plot that shows how much precip fell in an our as opposed to reflectivity. Takes a long time to generate so be patient with it. 

## Running the Notebooks

You can either run the notebook using [Binder](https://binder.projectpythia.org/) or on your local machine.

### Running on Binder

The simplest way to interact with a Jupyter Notebook is through
[Binder](https://binder.projectpythia.org/), which enables the execution of a
[Jupyter Book](https://jupyterbook.org) in the cloud. The details of how this works are not
important for now. All you need to know is how to launch a Pythia
Cookbooks chapter via Binder. Simply navigate your mouse to
the top right corner of the book chapter you are viewing and click
on the rocket ship icon, (see figure below), and be sure to select
“launch Binder”. After a moment you should be presented with a
notebook that you can interact with. I.e. you’ll be able to execute
and even change the example programs. You’ll see that the code cells
have no output at first, until you execute them by pressing
{kbd}`Shift`\+{kbd}`Enter`. Complete details on how to interact with
a live Jupyter notebook are described in [Getting Started with
Jupyter](https://foundations.projectpythia.org/foundations/getting-started-jupyter).

Note, not all Cookbook chapters are executable. If you do not see
the rocket ship icon, such as on this page, you are not viewing an
executable book chapter.


### Running on Your Own Machine

If you are interested in running this material locally on your computer, you will need to follow this workflow:


1. Clone the `https://github.com/ProjectPythia/proto-cookbook` repository:

   ```bash
    git clone https://github.com/ProjectPythia/proto-cookbook.git
   ```

1. Move into the `proto-cookbook` directory
   ```bash
   cd proto-cookbook
   ```
1. Create and activate your conda environment from the `environment.yml` file
   ```bash
   conda env create -f environment.yml
   conda activate cookbook-example
   ```
1. Move into the `notebooks` directory and start up Jupyterlab
   ```bash
   cd notebooks/
   jupyter lab
   ```
