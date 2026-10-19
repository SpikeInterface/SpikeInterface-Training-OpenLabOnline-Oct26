# SpikeInterface-Training-OpenLabOnline-Oct26

Material for SpikeInterface Tutorial @ Open Lab Online - October 2026

## Data

You can go through the notebooks in this course yourself, or code along with us on the day. To do so, please download `dandiset-000939-90s.zip` and `full_analyzer_lupin_000939.zarr.zip` from this Zenodo page: https://zenodo.org/records/23373455

This data was originally collated and organised for the [Ephys track](https://neuroinformatics.dev/open-software-summer-school/2026/extracellular-electrophysiology.html) of the [Open Software Summer School](https://neuroinformatics.dev/open-software-summer-school/index.html). You can read more about the data [here](https://neuroinformatics.dev/course_ephys_osss/course-data.html).


## Installation

We recommend that you [install uv](https://docs.astral.sh/uv/getting-started/installation/). This is an unbelievably good new package
management tool for Python.

Open your Terminal app and cd (change directory) to where you like to keep github repos. Then clone this repo, and navigate to the `notebooks` folder of it by entering the following commands into your Terminal:

``` shell
git clone https://github.com/SpikeInterface/SpikeInterface-Training-OpenLabOnline-Oct26.git
cd SpikeInterface-Training-OpenLabOnline-Oct26/notebooks/
```

Now open jupyter lab (you don't need to install this - uv will take care of it) using uv:

``` shell
uv run jupyter lab
```

Or if you prefer to use vscode:

``` shell
uv run code .
```

If you like traditional virtual environments, please visit [this page](https://github.com/SpikeInterface/spikeinterface/tree/main/installation_tips) to install on your laptop python+spikeinterface.


## Schedule

**October 19th - 15:00-18:00 CET**


### Introduction

Display installation instructions and check that everyone has the necessary software ready
while people are entering the room

1. Introduction to Spike Sorting
2. Introduction to `SpikeInterface` 
3. (mention various projects and papers)


**Hands on tutorials - 15:30-18:00**

-> Questions on chat <-

1. Reading + Manipulation (30 min - Chris)
    - Read and visualise data
    - The importance of probes
    - Splitting by channels 
    - (optional) Make your own probe

2. Preprocessing (30 min - Alessio)
    - Apply and visualize preprocessing 
      - filter
      - CMR
    - Detect bad channels
    - Saturation
    - Motion

3. Spike sort and Analysis(30 min - Chris)
    - Run a spike sorter (LUPIN)
    - Create a `SortingAnalyzer` to explore your sorting
    - Compute some extensions
    - Play with the extension outputs

4. Curate (45 min - Alessio)
    - GUI - manual curation
    - Automatic:
      - Simple, threshold-based curation
      - Curation using ML models / Bombcell
      - Merging units
    - Using GUI  + Automated curation
