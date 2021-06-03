# ProLIF-paper

Data and code for the ProLIF paper

## Description
---

- **Notebooks**  
  The `Analysis.ipynb` notebook, as well as a `pickles` subdirectory containing the
  pandas DataFrames generated during the analysis as binary pickle files (to avoid
  re-running the calculations)
- **Data**
  - `*.xlsx`: the annotated sequences of proteins, as downloaded from GPCRdb
  - `*.pqr`: PQR files downloaded from the PDB2PQR webserver
- **Figures**  
  All figures and interactive plots generated during the analysis

## Instructions
---

To simply read the notebook that was used to generate all data and figures in the paper,
we recommend following [this link](https://nbviewer.jupyter.org/github/chemosim-lab/ProLIF-paper/blob/main/Notebooks/Analysis.ipynb).

To run the notebook locally, you will first need to install some dependencies.

Start by cloning this repository:
```bash
git clone https://github.com/chemosim-lab/ProLIF-paper.git
cd ProLIF-paper
```

Then you can install the dependencies with `conda` and `pip` in a dedicated virtual
environment:

```bash
# install dependencies in a new virtual environment
conda env create --name prolif-paper --file environment.yml
# install prolif
conda activate prolif-paper
pip install https://github.com/chemosim-lab/ProLIF/archive/v0.3.1.zip
```

Once this is done, you should be able to run the [Analysis notebook](Notebooks/Analysis.ipynb):
```bash
jupyter-notebook Notebooks/Analysis.ipynb
```

## License
---

Unless otherwise noted, all files in this directory and all subdirectories are distributed under the Apache License, Version 2.0:
```
    Copyright 2021 Cédric BOUYSSET

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
```

