# Unlocking Your Photos: Building a Custom Image Classifier with CreateML - Resilient Coders

Learning Objective
    Image classification
    Build and Train Custom Image Classification
    Apply image recognition in real world problems

Machine Learning -
**Teaching** computers recognize patterns using data.
For image classification on fruits dataset -
    Model learns patterns from data - colour, texture, shape.
    It then makes predictions on new unseen data

Traditional vs ML classification.

    ML is flexible - adapts to variations without needing new rules (than traditional if-else or rules to define how a particular fruits lookings)
    Scalable - Handles more images, faster prediction

CreateML Apple Software Development tool:

    No need of deep AI knowledge
    Drag and drop interface
    Runs locally on Mac
    Optimized for Apple Devices
    Fast and efficient (Apples Metal Framework)

Core Features of Create ML

    Pre-configured models --
        Image Models        Motion Model
        Video Models        Sound Model
        Text Models         Tabular Data Model
        Spatial Model
        Object Models

XCode to be used for accessing CreateML

Break down the process-
    Collect and label - folder with the label of the image
    Ensure balanced dataset across class variables
    Use ImageNet or web scraping for datasets
    Train the machine learning model
    Evaluate Model Accuracy

Folder Structure--
                /xDataSet
                    /apples
                    /bananas
                    /grapes
                    /oranges
                    /strawberries

Parameters --
              Feature Extractor - Image Feature PrintV1
              Model availability - OS version compactibility
              Iteration
              Images Augmentation - add noise and increase the dataset size add modified versions of existing dataset - avoid overfitting

Recall - How many (#) of correctly identified entries
Precision - How well we are able to correctly identify entries

Exporting model - File ext .mlmodel

50X model traning - CreateML (Image classification)