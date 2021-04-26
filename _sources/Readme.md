To open in Jupyter: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/guiwitz/ImagingStats/f9f9450ca7091dd2a53aad9bd869840c565c14d7)

To open in Google Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/guiwitz/ImagingStats/blob/master)

To open in RStudio: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/guiwitz/ImagingStats/f9f9450ca7091dd2a53aad9bd869840c565c14d7?urlpath=rstudio)

# Imaging statistics

This is the repository containing the material for the Imaging statistics course given at Bern University in the frame of the Microscopy Imaging Center trainings. Material has been created by Guillaume Witz (Bern University, MIC-ScITS) and Maciej Dobrzynski (Bern University, Cellular Dynamics Lab). 

The course illustrates an image processing pipeline from data download to statistical analysis realized in Python and R. Notebooks can be run interactively either via the [mybinder](https://mybinder.org/) service or via Google Colab using the badges at the top of this Readme.

## Image processing

The image processing part of the course is done in Python. The [image_processing.ipynb](image_processing.ipynb) notebook presents a classical thresholding-based segmentation, and also highlights the "data science" aspects of an analysis pipeline like file parsing or extraction and organisation of extracted data into tables.

The [advanced_processing.ipynb](advanced_processing.ipynb) presents an alternative segmentation strategy and in particular shows how easy it can be to deploy Deep Learning based solutions in Python as done here with the segmentation algorithm [cellpose](http://www.cellpose.org/).

Both notebooks can be run on Binder and Google Colab. In particular the second one benefits from using the free GPU from Colab to run cellpose (cellpose might not work properly on Binder because of the limited RAM).

Finally the [image_processing.ipynb](rise_presentation/image_processing_rise.ipynb) notebook can also be run as a slide presentation via the [RISE](https://rise.readthedocs.io/en/stable/) package in Jupyter (e.g on binder) or directly in the browser at [this link](https://guiwitz.github.io/ImagingStats/image_processing_rise.slides.html#/).

## Statistical analysis

### Presentation

The presentation on basics statistics can be found as [HTML file](statsBasics.html) or [R markdown file](statsBasics.Rmd) in this repository. You can also directly access the presentation using [this link](https://guiwitz.github.io/ImagingStats/statsBasics.html#1).

### Notebooks

The statistical analysis of the data extracted in the image processing part are visible in multiple files names ```R_analysis```. The [R_analysis.Rmd](R_analysis.Rmd) can be executed directly in RStudio by using the appropriate binder badge (top of this document). The [R_analysis.ipynb](R_analysis.ipynb) notebook can be run either in Jupyter on Binder or directly in Colab. The possibility to run R on Colab is still experimental and a few bugs or package incompatibilities might remain.