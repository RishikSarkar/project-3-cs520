# CS 520 Project 3: Machine Learning - What Is It Good For?

## Authors:
Rishik Sarkar & Aditya Girish

## Description:
This repository contains our training, testing, and analysis code for 3 ML models to predict and improve our bot's grid-traversal performance.

## Project Structure:
- *Bot1.ipynb* contains our setup code for the bot
- *Model1.ipynb* contains the dataset generation code, model training, testing, and analysis for Model 1
- *Model2.ipynb* contains the dataset generation code, model training, testing, and analysis for Model 2
- *Model3.ipynb* contains the dataset generation code, model training, testing, and analysis for Model 3

## Additional Temporary Notes (for Aditya):
- I have currently created the *Bot1* and *Model1* notebooks, with *Bot1* containing the setup code to generate the 30x30 ship; place bot, crew, and alien; initialize sensors and probability matrices; update matrices; and move bots and aliens according to what we had in Project 2. It is unlikely that this will change much unless we find a significant bug with how probabilities are calculated.
- *Model1* has access to all the functions defined in *Bot1*, and runs the setup code beforehand. This process will be duplicated in *Model2* and *Model3*, with the only difference in dataset generation being the metrics. I am currently rerunning the Bot1 simulation with our Project 2 metrics to determine the best alpha and k-values, since they will be very important in increasing data quality. Here are some immediate changes that we can work on to start with:
    - The simulation method in *Model1* will be updated to include the metrics used in the generated dataset for ML training, after the alpha and k-values are determined
    - Similarly, the plot generation will be obsolete or will need to be completely changed
    - The dataset can be saved as a .csv file for later
    - We need to figure out the answers to the questions posed in the assignment before we decide the metrics to use
