[![Contributors][contributors-shield]][contributors-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.11361363.svg)](https://doi.org/10.5281/zenodo.11361363)

[contributors-shield]: https://img.shields.io/github/contributors/nih-sparc/sparc-marker-paper.svg?style=flat-square
[contributors-url]: https://github.com/nih-sparc/sparc-marker-paper/graphs/contributors
[stars-shield]: https://img.shields.io/github/stars/nih-sparc/sparc-marker-paper.svg?style=flat-square
[stars-url]: https://github.com/nih-sparc/sparc-marker-paper/stargazers
[issues-shield]: https://img.shields.io/github/issues/nih-sparc/sparc-marker-paper.svg?style=flat-square
[issues-url]: https://github.com/nih-sparc/sparc-marker-paper/issues
[license-shield]: https://img.shields.io/github/license/nih-sparc/sparc-marker-paper.svg?style=flat-square
[license-url]: https://github.com/nih-sparc/sparc-marker-paper/blob/master/LICENSE

# Code: SPARC Marker Paper

## About
This is the code associated with the SPARC Marker Paper. SPARC is one of the NIH Common Fund's Program that seeks to accelerate the development of therapeutic devices that modulate electrical activity in the ANS to improve internal organ functions and suppress dysfunction. The SPARC Marker paper currently being prepared is aimed at providing an overview of the SPARC program, presenting its major outcomes, and giving an assessment of the impact of the program on bioelectronic medicine-related research and development. The repository contains the jupyter notebook developed to analyze data for the paper and generate figures.


## Standards followed
The overall code is structured according to the [FAIR-BioRS guidelines](https://fair-biors.org/). The Python code in the Jupyter notebook [main.ipynb](main.ipynb) follows the [PEP8 guidelines](https://peps.python.org/pep-0008). Functions are documented with docstring formatted following [Google's style guide](https://google.github.io/styleguide/pyguide.html#38-comments-and-docstrings). All the dependencies are documented in the [environment.yml](environment.yml) file.

## Using the Jupyter notebook

### Prerequisites 
We recommend using Anaconda to create and manage your development environment and using JupyterLab to run the notebook. All the subsequent instructions are provided assuming you are using [Anaconda (Python 3 version)](https://www.anaconda.com/products/individual) and JupyterLab.

### Clone repo
Clone the repo or download as a zip and extract.

### cd into the code folder

Open Anaconda prompt (Windows) or the system Command line interface then naviguate to the code
```sh
cd .sparc-marker-paper

```

### Setup conda env
```sh
$ conda env create -f environment.yml
```

### Setup kernell for Jupyter lab
```sh
$ conda activate sparc-marker-paper
$ conda install ipykernel
$ ipython kernel install --user --name=<any_name_for_kernel>
$ conda deactivate
```
### Launch Jupyter lab
Launch Jupyter lab and naviguate to open the main.ipynb file. Make sure to change the kernel to the one created above (e.g., see [here](https://doc.cocalc.com/howto/jupyter-kernel-selection.html#cocalc-s-jupyter-notebook)). We recommend to use the [JupyterLab code formatter](https://github.com/ryantam626/jupyterlab_code_formatter) along with the [Black](https://github.com/psf/black) and [isort](https://github.com/PyCQA/isort) formatters to facilitate compliance with PEP8 if you are editing the notebook.

## Inputs/outputs

The Jupyter notebook makes use of files in the dataset associated with the SPARC Marker Paper [(see here)](https://github.com/nih-sparc/sparc-marker-paper-inventory). You will need to download the dataset at add it in the input folder.

Outputs of the code include tables displayed directly in the notebook and plots displayed in the notebook but also saved as files. These saved plot files are included in the [output](output) folder here. 

## License
This work is licensed under
[MIT](https://opensource.org/licenses/mit). See [LICENSE](LICENSE) for more information.

## Feedback and contribution
Use the [GitHub issues](https://github.com/nih-sparc/sparc-marker-paper/issues) for submitting feedback or making suggestions. You can also work the repository and submit a pull request with suggestions.

## How to cite
If you use this code, please cite the SPARC Marker Paper (it will be listed [here]() when available) and also cite this repository as:

```bash
Patel, Bhavesh. Code: SPARC Marker Paper [Software]. Zenodo. https://doi.org/10.5281/zenodo.11361363
```
