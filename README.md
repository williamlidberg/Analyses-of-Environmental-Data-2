[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Twitter Follow](https://img.shields.io/twitter/follow/William_Lidberg?style=social)](https://twitter.com/william_lidberg)

# Analyses-of-Environmental-Data-2

The course focuses on applying statistical models and machine learning methods to spatial data. The course will cover four topics:\
**1 Setting up your analytical envrionment** \
**1 Acquiring and wrangling real data** \
**2 Processing of spatial data with open source software** \
**3 Topographical modeling**  
**4 Implementing machine learning models on spatial data** 

After completing the course, the student should be able to:
*	Collect and prepare forest data from authorities such as the Swedish Forestry Agency and the Swedish Environmental Protection Agency for analysis.
*	Independently perform spatial modeling of forest land based on remote sensing data.
*	Identify and classify differences and similarities between statistics and machine learning for ecological data.
*	Compare some traditional machine learning models based on accuracy and calculation speed.
*	Combine machine learning with geographic data to produce maps of biological conditions for sustainable forestry.

# Table of  Contents
M1: setting upp your environment
M2: Introduction to Python
M3: Data wrangling
M4: Topographical modeling
M5: Geopandas
M6: Satellite imagery
M7: Machine learning on vector data
M8: Machine learning on raster data
M9: Deep learning
1. [Setting up your analytical envrionment](#Setting-up-your-analytical-envrionment)
   1. [Jupyter notebooks](##Jupyter-notebooks) 
         1. [With google colab](###with-google-colab) 
         2. [With your own hardware](###with-your-own-hardware)
   2. 
   3. [Qgis](##Qgis)
2. [Introduction to Python](#Introduction-to-Python)
   1. [Vector data](##Vector-data)

   2. [Raster data](##Raster-data)
      1. [Rasterio](##Rasterio)
      2. [Xarray](##xarray)

3. [Data wrangling](#Data-wrangling)

4. [Topographical modeling](#Topographical-modeling)

5. [Geopandas](#Geopandas)

6. [Satellite imagery](#Satelite-imagery)

      1. [Geemap](###Geemap)
7. [Machine learning on vector data](#Machine-learning-on-vector-data)
8. [Machine learning on raster data](#Machine-learning-on-raster-data)
9. [Deep learning](#Deep-learning)
# Setting up your analytical environment
This course will only focus on free and open source tools which will always be accecible to you so you don't have to fight with the IT-department of your future employer. You will not need to pay for, or manage, expensive licens fees. In the first half of this course you used Rstudio to run R scripts but in order to work with Python scripts you need a Python envrinoment. 
## Jupyter notebooks
 Instead of Rstudio we will use Jupyter notebooks to analyze and interract with the data. The Jupyter Notebook is a web application for creating and sharing computational documents. It offers a simple, streamlined, document-centric experience. It supports over 40 programming languages, including Python, R, Julia, and Scala. In this crouse we will demonstrate two ways to set up notebooks. The easy way using google colab, and the fun way using your own computer.

The assignment for this module is to set up your analytical environment and install the following python packages:
* [Whitebox](https://pypi.org/project/whitebox/)
*


Once set up you need to run this code and report the 

### With google colab
Colab is a hosted Jupyter Notebook service that requires no setup to use and provides free access to computing resources, including GPUs and TPUs. All exercises in this course can be completed using google colab. However, colab is also quite slow due to limited hardware resources with about two processing cores and 12 GB of RAM. In order to get started with google colab you will need a google account and set up google drive for permanent storage. 

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/williamlidberg/Analyses-of-Environmental-Data-2/blob/main/Geopandas.ipynb)


### With your own hardware
Real geospatial datasets are rappidly expanding in both scope and detail which requires more processing power to handle. In addition your future employer might not be to happy if you upload senstive data to google colab/drive. Therefore I strongly recomend that you learn how to set up your analytical environment on local hardware. As a bonus, you can finally motivate paying a premium for that fancy computer.

To get started you need to download and install [Anaconda](https://www.anaconda.com/download). Follow the instructions and accept all defaults. Once installed you can open Anaconda and it should look something like this. 

<img src="images/navigator.png" alt="Study area" width="75%"/>

Look for the "create" button in the bottom and press it to create your first viritual environment. Once created the next step is to activate that enviromnet and going to "Home". Once on the Home screen you can select and install jupyter for your new environment. 

<img src="images/install.png" alt="Study area" width="75%"/>

Once installed you can go back to the "environments" tab and click the green arrow next to your envrionment. Select "open with jupyter notebook".
<img src="images/open_notebook.png" alt="Study area" width="75%"/>

you will then be greeted by a webpage with a little button in the top right corner saying "new". Click itt and select "python 3 ipykernel". Now you have set up a analytical envrionment on your own hardware. 
<img src="images/new_notebook.png" alt="Study area" width="75%"/>

Enter the following lines in the first cell and run it to see how good your computer is:\
import multiprocessing\
cores = multiprocessing.cpu_count()\
cores

If the number of cores is less than four you should use google colab. You should also look for a new computer.  
# Processing of spatial data with open source software
## Vector data
### Geopandas
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/williamlidberg/Analyses-of-Environmental-Data-2/blob/main/Geopandas.ipynb)
### Rasterio
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/williamlidberg/Analyses-of-Environmental-Data-2/blob/main/Geopandas.ipynb)
### Xarray
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/williamlidberg/Analyses-of-Environmental-Data-2/blob/main/Geopandas.ipynb)
## Raster data

## Satellite data
### Geemap
 [Google earth Engine (GEE)](https://earthengine.google.com/) has become very popular in the geospatial community and it has empowered numerous environmental applications at local, regional, and global scales. [Geeemap](https://geemap.org/) is built upon ipyleaflet and ipywidgets, and enables users to analyze and visualize Earth Engine datasets interactively within a Jupyter-based environment.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/williamlidberg/Analyses-of-Environmental-Data-2/blob/main/Geopandas.ipynb)
# Topographical modeling
## Whittebox Tools
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/williamlidberg/Analyses-of-Environmental-Data-2/blob/main/Geopandas.ipynb)
# Machine learning with spatial data
## Random Forest
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/williamlidberg/Analyses-of-Environmental-Data-2/blob/main/Geopandas.ipynb)
## Deep learning
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/williamlidberg/Analyses-of-Environmental-Data-2/blob/main/Geopandas.ipynb)
