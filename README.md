# FinalProject1-CIS1051
CIS 1051 Final Project for Spring 2023 

Title: fMRI Analysis Using Nilearn
Name: Caedyn Lipovsky
Year: Sophomore

Youtube Video URL: 
https://www.youtube.com/watch?v=Navkcr5mJmk


Introduction: 

This project was a very long and difficult process for me. With most projects, I start off overly ambitious, and this project was no different. I thought I could learn machine learning in a month as a intro to python student. 
Despite my overly ambitious nature, I was still determined to learn something related to AI and health. As a pre-med student, I am very interested in the intersection of technology and medicine. 
After doing some research for about a week, I realized it would be nearly imposible to just learn machine learning like that. However, I found that one topic that had a lot of resources and research was fMRI analysis. 
After doing some more research, I found Nilearn. This is a tool specifically geared towards analyzing fMRI images and conducting statistical analysis on brain imaging data with machine learning. I spent a few days trying to understand everything I was reading and downloading the many required modules. 
Due to the amount of research I had to do, I started my project late. However, once I felt confident to start, I began to understand it more. 

The data: 

Using OpenNeuro, a public neuroimaging database, I found data from a research conducted to analyze cognitive function of Parkinson's patients. The data collected fMRI images from 58 participants, age 55+. The researchers of this study also used fMRI images of participants with normal cognitive function, and Parkinson's patients with dementia and mild impairment. 
The data included participant descriptions (age,sex,handedness,years of education), established cognitive tests (MOCA, for example), and other tests (visuospatial, memory...). 
In order to save both storage and time, I selected 10 participants with ranges of cognitive test scores. However, I focused on two participants with scores on the extreme ends (highest and lowest). 

The goal of the project: 

The goal of my project was to compare healthy brains with diseased, Parkinson's brains using Nilearn. Before, I could even establish a model, however, I needed to pre-process the brain images. 
The best possible outcome was to create a machine learning model that would utilize training and testing data to help physicians determine susceptibility to developing Parkinson's disease based on cognitive function. Although, I did not achieve this, this project made me very interested in this methodology, and I hope to utilize this in my future career/research. 

The Process: 
To start, I utilized the Userguide on the Nilearn website. This guide was extremely comprehensive and is actually made to help students conduct fMRI analysis on their own. 
I first started with attempting to do basic codes. I imported my data and stored it in its own file titled cisdata. I also imported the Harvard Oxford Brain Atlas as a standard for what my images should look like. 
Then I imported all of the CSV files and printed them in a tabular format.
Then, I utilized separate lines to plot the fMRI images for each 10 subjects that I had chosen. 
Before I did this, however, it was necessary to pre-process all of the images. For subject 1, you can see a distinct comparison of the non-mean images and the mean images. For these fMRI images, the images were in 4D meaning 4-coordinates (x,y,z,t), t representing a time-step. Thus all images needed to be transformed from 4D to 3D using the mean image function found on Nilearn. 
For each subject, I found the mean image to make all fMRI's easier to understand. However, there was some difficulty for some of the images. 
Because I wanted to focus on patient 2 and 10, I did the rest of the pre-processing steps for them. I first smoothed all of the brain images. This made it so you could noticeably see the Regions of Interests (ROIs). Then for subjects 2 and 10, I applied a mask. This was done in order to outline the areas of interest on the meaned brain images. 
For subject 2, I started to conduct Support Vector Machine analysis, but ultimately was struggling immensely with this since I have no prior knowledge of linear algebra or computational statistics. 

Difficulties: 
- Overwhelming amount of information that was extremely difficult to dissect and undestand
- No prior knowledge of linear algebra made this all VERY difficult to do
- I needed the perfect type of data to analyze (had to be between-patient data not within-patient data, needed to have an independent and depdent variable, and had to include functional MRI images). I didn't figure this out until after I had processed some of my images, so I had to re-download a lot of data from OpenNeuro. 
- I had to figure out what modules and libraries were required to do what I wanted to do
- I used anatomical images (instead of functional) at first which did not work well with a lot of Nilearn's analysis methods
- Worst struggle of them all was feeling like I was spending hours on one thing and thinking I wasn't going to get anywhere with the project 


Best Part of the Process: 

Realizing how interested I am in learning more about how AI can be applied to issues in medicine! 



Sources: 
https://main-educational.github.io/brain_encoding_decoding/svm_decoding.html
https://carpentries-incubator.github.io/SDC-BIDS-fMRI/aio/index.html
https://openneuro.org/datasets/ds004392/versions/1.0.0
https://nilearn.github.io/dev/quickstart.html
https://www.analyticsvidhya.com/blog/2017/09/understaing-support-vector-machine-example-code/#How_to_Implement_SVM_in_Python_and_R?
https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6666603/
https://www.andysbrainblog.com/videos
https://www.youtube.com/watch?v=4FVGn8vodkc
https://brainiak.org/tutorials/02-data-handling/
https://dartbrains.org/content/Introduction_to_Neuroimaging_Data.html
https://lukas-snoek.com/NI-edu/fMRI-introduction/week_1/python_for_mri.html
https://medium.com/coinmonks/visualizing-brain-imaging-data-fmri-with-python-e1d0358d9dba
https://www.kaggle.com/code
