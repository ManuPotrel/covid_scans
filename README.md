# Covid Project

## Context

This project started in early 2021, in the middle of the pandemic. The goal here is to train a model to recognize patterns on chest radiographs that would enable the identification of a Covid-19 infection.

## Data

The data used here is the <a href="https://www.kaggle.com/tawsifurrahman/covid19-radiography-database">Kaggle Covid-19 Radiography Database</a> (since then, the database has been updated with more than 10,000 new images).

## Analysis

The data is very biased. Simple models are able to reach more than 85% in accuracy after a dimensionality reduction.<br>
The Covid patients' scans can be distinguished very easily by a non expert human being (quality of the image, presence of tubes).<br>
The Normal and Viral Pneumonia patients are all children, inducing a different frame. Furthermore, they're holding their arms up.

## Experimentation

Many different preprocessings have been tried to fight off those biases, with very limited success.

## Classification

You will find four different CNN models here, two relatively simple ones and two inspired by the VGG-16 architecture (one non-preprocessed and one preprocessed each). As expected, the accuracy is suspiciously outstanding and the Grad-CAMs (interpretability) don't impress.

## Deployment

In the deployment folder, you will find our streamlit application, which will enable the online testing of the models.

## Requirements

You will need to download the data yourself at the link given above.<br>
If you want to experiment with the U-Net model that was tried, you will need to download (or train) your own weights.<br>
To see the full streamlit app, you may need to build your own dataframes.
