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

# 📚 Table of Contents

### Module Overview
- [Module 1: Setting up your environment](#setting-up-your-environment)
    - [Jupyter notebooks with google colab](#Jupyter-notebooks-with-google-colab)
    - [Jupyter notebooks with your own hardware](#Jupyter-notebooks-with-your-own-hardware)
- [Introduction to python](#introduction-to-python)
  - [Module 2: Basic commands](#basic-commands)
  - [Module 3: Data wrangling](#data-wrangling)
- [Geospatial processing](#geospatial-processing)
  - [Module 4 Raster data](#raster-data)
  - [Module 5 Sattelite data](#sattelite-data)
  - [Module 6 Vector data](#vector-data)
- [Machine learning on geospatial data](#machine-learning-on-geospatial-data)
  - [Module 7 Machine learning on vector data](#machine-learning-on-vector-data)
  - [Module 8 Machine learning on raster data](#machine-learning-on-raster-data)
  - [Module 9 Deep learning](#deep-learning)
- [Module 10: Web mapping](#web-mapping)



# 💻 Setting up your environment

This course will only focus on free and open source tools which will always be accecible to you so you don't have to fight with the IT-department of your future employer. You will not need to pay for, or manage, expensive licens fees. In the first half of this course you used Rstudio to run R scripts but in order to work with Python scripts you need a Python envrinoment. 
## Jupyter notebooks
 Instead of Rstudio we will use Jupyter notebooks to analyze and interract with the data. The Jupyter Notebook is a web application for creating and sharing computational documents. It offers a simple, streamlined, document-centric experience. It supports over 40 programming languages, including Python, R, Julia, and Scala. In this crouse we will demonstrate two ways to set up notebooks. The easy way using google colab, and the fun way using your own computer.



### Jupyter notebooks with google colab
Colab is a hosted Jupyter Notebook service that requires no setup to use and provides free access to computing resources, including GPUs and TPUs. All exercises in this course can be completed using google colab. However, colab is also quite slow due to limited hardware resources with about two processing cores and 12 GB of RAM. In order to get started with google colab you will need a google account and set up google drive for permanent storage. 

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/williamlidberg/Analyses-of-Environmental-Data-2/blob/main/modules/module_1/Assignment_1.ipynb)


### Jupyter notebooks with your own hardware
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
# 🐍 Introduction to python
Learn the foundational syntax and structures of Python programming, tailored for geospatial analysis.
## Basic commands
This module introduces Python basics such as variables, loops, conditionals, and functions—skills essential for scripting and automation.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/williamlidberg/Analyses-of-Environmental-Data-2/blob/main/modules/module_2/Assignment_2.ipynb)

## Data wrangling
Explore how to clean, transform, and manipulate real-world data using libraries like pandas to prepare datasets for analysis.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/williamlidberg/Analyses-of-Environmental-Data-2/blob/main/modules/module_3/Assignment_3.ipynb)

# 🌍 Geospatial processing
Work with geospatial data formats and understand how to extract insights from raster and vector data.
## Raster data
Learn to handle raster datasets (such as elevation models and satellite imagery) using rasterio and numpy.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/williamlidberg/Analyses-of-Environmental-Data-2/blob/main/modules/module_4/Assignment_4.ipynb)

## Sattelite data
Process and visualize satellite imagery, and explore spectral bands to analyze landscape features.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/williamlidberg/Analyses-of-Environmental-Data-2/blob/main/modules/module_5/Assignment_5.ipynb)
## Vector data
Manipulate shapefiles and other vector formats using geopandas, and perform spatial joins and filtering.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/williamlidberg/Analyses-of-Environmental-Data-2/blob/main/modules/module_6/Assignment_6.ipynb)


# ⚙️ Machine learning on geospatial data
Apply machine learning techniques to spatial datasets for classification, regression, and prediction.
## Machine learning on vector data
Use traditional machine learning models like Random Forest and SVM to classify vector-based ecological data.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/williamlidberg/Analyses-of-Environmental-Data-2/blob/main/modules/module_7/Assignment_7.ipynb)

## Machine learning on raster data
Train models on raster datasets to produce spatial predictions and thematic maps.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/williamlidberg/Analyses-of-Environmental-Data-2/blob/main/modules/module_8/Assignment_8.ipynb)

## Deep learning
Introduce deep learning for geospatial analysis using CNNs, with examples using image data and spatial grids.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/williamlidberg/Analyses-of-Environmental-Data-2/blob/main/modules/module_9/Assignment_9.ipynb)

# 🗺️ Web mapping
Learn to publish interactive maps using Python libraries like folium and geemap, and share results online.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/williamlidberg/Analyses-of-Environmental-Data-2/blob/main/modules/module_10/Assignment_10.ipynb)


