# Project 5: Unsupervised Learning (k-Means and EM)

CS-4103 Fundamentals of Machine Learning, University of Tulsa

## What is here

- `assignment/Assignment 5.ipynb`, the notebook you complete. It covers k-Means and expectation maximization on synthetic Gaussian mixtures, customer segmentation on real sales data, and image compression with k-Means.
- `data/online_retail_customers.csv`, one row per customer of an online shop, for the customer segmentation part.
- `data/imgs/`, one sample image for the compression part. Add your own 5 images here.
- `assignment/Project 5 - Unsupervised Learning, k-Means and EM.pdf`, the project spec. The same PDF is posted on Harvey.

Source: `online_retail_customers.csv` is built from the [Online Retail](https://archive.ics.uci.edu/dataset/352/online+retail) dataset (Daqing Chen, UCI Machine Learning Repository, 2015, CC BY 4.0). It keeps completed sales by known customers and summarizes them as one row per customer: the days since their last order, their number of orders, and their total spend in pounds sterling.

## Running in Colab

Run the notebook in Google Colab. It does not need a GPU.

- [Assignment 5 in Colab](https://colab.research.google.com/github/zacharytgray/fund-ml-project-5/blob/main/assignment/Assignment%205.ipynb)

After you open it, save your own copy with **File > Save a copy in Drive** and work in that copy. Run the first code cell every time you open the notebook: it copies this repository onto the Colab machine so the notebook finds `../data`.

For the image compression part in Colab, open the **Files** panel on the left and upload your images into `fund-ml-project-5/data/imgs`. Uploads are lost when the Colab machine shuts down, so keep your own copies.

## Running on your own computer

Use Python 3.10 or newer.

    pip install -r requirements.txt
    jupyter notebook

Open the notebook from the `assignment` folder. It loads data through `../data`, so it fails if you move it or start it elsewhere.

## Working in the notebook

Both models in this project come from scikit-learn: `KMeans` and `GaussianMixture`. The data loading, the synthetic datasets, the repeated runs and their scoring, and the plots are already written. Your job is to build and configure each model, read the learned parameters out of the fitted models, choose the number of customer segments, and write about what you see.

Fill in each `TODO`. The numbered comment above a `TODO` lists the steps that region needs.

Import nothing beyond the libraries listed in the import cell.

Run every cell, top to bottom, before you submit.

## Submitting

Submit through Harvey:

- The notebook, with all outputs visible. In Colab, download it with **File > Download > Download .ipynb**.
- The report PDF described in the spec.

A notebook with cleared outputs is graded as though the code did not run.
