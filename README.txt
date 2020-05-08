*****COVID-19 X-rays predictions

This Notebook is using a CNN and a RF to classify X-ray images as covid19-positive or covid19-negative. it is using data from 2\ kaggle datasets :
1- https://www.kaggle.com/bachrr/covid-chest-xray
2-https://www.kaggle.com/tawsifurrahman/covid19-radiography-database


****Team
    -Aya Lahlou
    -Elarbi Amraoui
    -Huangrui Chu
    -Cullen Peters
    
****Personal Work

I started with the data extraction,cleaning,visualization, and analysis of the first dataset. I then pre-processed its images.
When we added the second dataset, I applied the same image pre-processing from dataset-1.  I then moved on to the creation of a
CNN model, and talked with the team about the best metric to choose. I then created some helper functions for the CNN and
started designing models.After designing multiple models and finetuning them and kept four of them in this notebook, which I 
consider were important milestones-- each one encovers a new limitation. Then after Aya found that her Random Forest was biased 
towards the sides of her model and wasn’t extracting information from the lungs. I designed a crop function for the images and 
decided to train the last model one more time on the copped images. I did that because I tried many visualizations of features 
importance to try to see what does my CNN model ‘see’, but they didn’t work as expected, so as I precaution I had to crop them 
and retrain the last model, I then made a soft voting between two of the CNNs, and then another one between those two CNNs and 
Aya's Random Forest.
