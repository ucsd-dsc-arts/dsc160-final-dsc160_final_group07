# Project Title

DSC160 Data Science and the Arts - Final Project - Generative Arts - Spring 2020

Project Team Members: 
- Kevin Elkin, kelkin@ucsd.edu
- Liam McCarthy, lamccart@ucsd.edu
- Umang Saraf, usaraf@ucsd.edu
- Charul Sharma, c4sharma@ucsd.edu
- Karan Sunil, ksunil@ucsd.edu

## Abstract

(10 points) 

Our concept is to create a generative image from any query a user inputs by scraping the top 50 results for that query from an engine such as Google Images. Next, we will use these images in our model (GAN) to create something that accurately depicts the words/phrases entered in the search engine. For instance, if we entered the phrase “Green Birds Flying” or “Bay Area” we would obtain the top 50 images from google images, web scrape them, and then fit them in our model, and then produce an all encompassing image that has been generated based on the training images passed in. We will then be able to create a gallery of our results on a website for different words and phrases. We are hoping to capture multiple ideas and items within one photo; an example of this would pertain to culture. Culture itself can often be very complex and have various aspects to it such as people, food, country of origin, habits, hobbies, etc. We will attempt to capture something that has this level of granularity into one condensed image (stretch goal). 


We will be using Generative adversarial networks (GAN) to help generate the images. As of now, we are still actively conducting research to determine what other approaches we can take to accomplish this task (and examine how others have achieved a similar result). As of now, we have been reading through the implementation posted here on the CIFAR10 dataset.  https://machinelearningmastery.com/how-to-develop-a-generative-adversarial-network-for-a-cifar-10-small-object-photographs-from-scratch/

Please let us know if you have any guidance or suggestions as to how we can best approach this problem. 

We will build a web scraper to download the top 50 results from an input query string. The training data will be formatted as jpegs. 


We hope that the final image will be a good representation of the different search results. This will almost be like a summary image of the keyword entered by the user. This will take the complexity of multiple different images and simplify it down to one image for the user to view. 

Website - we will have a gallery of different keywords and the respective generative images. We will also give the user the option to create a generative image real time. They will enter their search query into a textbox and we will do the web scraping and generate the representative image.

The first challenge that will arise is attempting to scrape Google image search results to get the images that are received. This will involve having queries for different keywords or keyphrases which may be difficult to achieve and the scraping of the results of these queries may be computationally expensive. Moreover, we will have to download these images in mass quantities for the various generative art pieces and the downloading of the image results may take an extensive amount of space so we will have to make sure these are converted properly and stored on the server in an efficient manner. Additionally, another challenge will be the implementing a GAN model that will create new images off the original image data. These original images may be different sizes and resolution so there may be some preprocessing before inputting the images into the model. 

We will be using the idea of GANs covered in class. We will create a generator from latent vectors (code) to visual outputs. 

This is culturally interesting because since we are sourcing our images from the top query results, the final image will likely represent many facets of how our culture defines that word. We could expect a word such as “bat” to turn up some kind of combination of the weapon and animal, and could learn a lot about the defining images our culture considers when searching for a location (for example, a search for San Francisco will likely produce the golden gate bridge, not the tenderloin).

https://www.shvembldr.com/ - An interactive generative art piece created using computer algorithms and random seed as well as user input.
https://www.artbreeder.com/ - A GAN that breeds two images to create novel new ones using GANBreeder.
https://runwayml.com/ - An easy, code-free tool that makes it simple to experiment with machine learning models in creative ways.


## Data and Model

(10 points) 

In the final submission, this section will describe both the data you use for this project and any pre-existing models/neural nets. For each you should provide the name, a textual description, and a link. If there is a paper (for neural net) link that as well.
- Such and such Neural Net. The short description of this neural net. 
  - [link to code]().
  - [Title of Paper with Link](). 
- Training data. Short description of training data including bibliographic info. [link to data]().

## Code

(20 points)

This section will link to the various code for your project (stored within this repository). Your code should be executable on datahub, should we choose to replicate your result. This includes code for: 

- code for data acquisition/scraping
- code for preprocessing
- training code (if appropriate)
- generative methods

Link each of these items to your .ipynb or .py files within this seection, and provide a brief explanation of what the code does. Reading this section we should have a sense of how to run your code.

## Results

(30 points) 

This section should summarize your results and will embed links to documentation to significant outputs. This should document both process and show artistic results. This can include figures, sound files, videos, bitmaps, as appropriate to your generative art idea. Each result should include a brief textual description, and all should be listed below: 

- image files (`.jpg`, `.png` or whatever else is appropriate)
- audio files (`.wav`, `.mp3`)
- written text as `.pdf`

## Discussion

(30 points, three to five paragraphs)

The first paragraph should be a short summary describing your results.

The subsequent paragraphs could address questions including:
- Why is this culturally innovative?
- How does your generative computational approach differ from traditional art/music/cultural production? 
- How do your results relate to broader social, cultural, economic political, etc., issues? 
- What are the ethical concerns for this form of generative art? 
- In what future directions could you expand this work?

## Team Roles

Provide an account of individual members and their efforts/contributions to the specific tasks you accomplished.

## Technical Notes and Dependencies

Any implementation details or notes we need to repeat your work. 
- Additional libraries you are using for this project
- Does this code require other pip packages, software, etc?
- Does this code need to run on some other (non-datahub) platform? (CoLab, etc.)

## Reference

All references to papers, techniques, previous work, repositories you used should be collected at the bottom:
- Papers
- Repositories
- Blog posts
