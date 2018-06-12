![c2sm logo](./figures/c2sm.png)

# pyvis - Python Visualisation Course - c2sm - version 2


* Mathias Hauser ([ETHZ](http://www.iac.ethz.ch/people-iac/person-detail.html?persid=146568), [github](https://github.com/mathause)) <mathias.hauser@env.ethz.ch>
* Tarun Chadha  ([ETHZ](https://www.ethz.ch/services/en/organisation/departments/it-services/people/person-detail.html?persid=166149), [github](https://github.com/chadhat)) <tarun.chadha@id.ethz.ch>


## Format

The lectures consist of IPython Notebooks.

## Audience

Python beginners who should have programming experience in other
languages. Most examples and exercises are drawn from the field
of Climate Reseach.

## Duration

It's envisioned as a two day course.


## How to use it

### 1 Obtain the course material

Clone the git repository:

~~~~bash
git clone https://github.com/C2SM/pyvis.git
~~~~

Alternatively, you can download the [zip-archive](https://github.com/C2SM/pyvis/archive/master.zip)
and unpack.


### 2 Start jupyter notebook

#### Computer room at ETH (HG D 12)

<details>
<summary>Click for details</summary>

 * log in to Fedora (you may have to reboot the computer)
 * execute the following commands:

~~~~bash
export CONDA_ENVS_PATH=/opt/kunden/hauser/conda/envs
source activate pyvis
# go to the directory of the material
jupyter notebook
~~~~

</details>

#### At IAC ETH (on linux computers)

<details>
<summary>Click for details</summary>

 * you can use the standard conda environment
 * execute the following commands:

~~~~bash
module load conda/2018
source activate iacpy3_2018
# go to the directory of the material
jupyter notebook
~~~~

See also the [Python FAQ on the IAC wiki](https://wiki.iac.ethz.ch/IT/PythonFAQ) (restricted access).

</details>

#### On your personal computer

<details>
<summary>Click for details</summary>

 * Follow the [conda installation guide](https://conda.io/docs/user-guide/install/) for your operating system.
 * Download the `packages.yml` file 
   * Go to [`packages.yml`](https://github.com/C2SM/pyvis/blob/master/packages.yml)
   * right click on the `Raw` button
   * Save File As...
 * Install the environment and open jupyter notebook

##### From the command line

<details>
<summary>Click for details</summary>

~~~~bash
conda env create -f packages.yml
~~~~
 * open jupyter notebook 

~~~~bash
source activate pyvis
# go to the directory of the material
jupyter notebook
~~~~

</details>

##### From Anaconda Navigator (Windows)

<details>
<summary>Click for details</summary>

 * Open Anaconda Navigator
 * Go to `Environments`
 * Select Import
   * Name: pyvis
   * Specification File: Select the `packages.yml` file
   * This will take about 20 minutes.
 * Go to `Home`
 * Switch to pyvis environment; Select `Applications on 'pyvis'`
 * Launch jupyter notebook
 * Go to the directory of the material

</details>

</details>


### 3 Hide Solutions

To hide the solutions a jupyter extension must be active. On the main page, click on `Nbextensions`. Then make sure `Hide input` has a tick.


### 4  Select the Course part

 * Part 0: very short introductions to Jupyter Notebooks, numpy, netCDF4, xarray, and pandas
 * Part 1: Introduction to matplotlib
 * Part 2: Some advanced feature of matplotlib and seaborn.
 * Part 3: Plotting georeferenced data with cartopy.
 * Part 4: Advanced exercises with plots contributed by the community.

## What's New

 * See [version history](./WHATS_NEW.md)


## Feedback

I would be very happy to hear from you (mail to <mathias.hauser@env.ethz.ch>).

Particularly welcome are problem reports, errors, criticism.

# License

Copyright (C) 2018 C2SM / Mathias Hauser / Tarun Chadha

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see [http://www.gnu.org/licenses/].
