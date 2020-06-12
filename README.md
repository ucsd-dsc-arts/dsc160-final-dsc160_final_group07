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
According to a recent study, in 18 major museums, 85% of the artists were white and 87% of artists were female. African American artists only had 1.2% of their paintings in these museums. While LatinX and Hispanic artists had just 2.8% of the paintings in the museums. Given that art is a field that has been around for thousands of years, this was quite surpring to learn about. We wanted to help reduce the gap between lesser represented communities in art. To do that we created some generative art for 10 prominent African American artists. 


We obtained paintings for different African American artists using wikiart. Next, we used these images to train a model (GAN) to create images that accurately depicts the different artwork of a given artist. We created a gallery of our results on a website for 10 different African American artists. We are hoping to capture general trends that are common to African American artists and capture multiple ideas and items within the artwork we scraped for an artist


We will be using Generative adversarial networks (GAN) to help generate the images. As of now, we are still actively conducting research to determine what other approaches we can take to accomplish this task (and examine how others have achieved a similar result). As of now, we have been reading through the implementation posted here on the CIFAR10 dataset.  https://machinelearningmastery.com/how-to-develop-a-generative-adversarial-network-for-a-cifar-10-small-object-photographs-from-scratch/

We will use wikiart to scrape images for 10 different African American artists. We aimed to get 20 images per artists. The training data will be formatted as jpegs and resized so that all images are of the same dimension. 


We hope that the final image will be a good representation of the different artists. This will almost be like a summary image to represent the artist. This will take the complexity of multiple different images and simplify it down to one image for the user to view. 

Website - we will have a gallery of different African American artists and the respective generative images. 

The first challenge that we faced was attempting to scrape artwork of African American artists. There were far fewer paintings on wikiart of African American artists than White artists. 

Additionally, another challenge will be the implementing a GAN model that will create new images off the original image data. These original images may be different sizes and resolution so there may be some preprocessing before inputting the images into the model. 

We will be using the idea of GANs covered in class. We will create a generator from latent vectors (code) to visual outputs. 
This is culturally important because African American artists are currently underrepresented in the generative art field and we would like to help change this. 

- https://www.shvembldr.com/ - An interactive generative art piece created using computer algorithms and random seed as well as user input.
- https://www.artbreeder.com/ - A GAN that breeds two images to create novel new ones using GANBreeder.
- https://runwayml.com/ - An easy, code-free tool that makes it simple to experiment with machine learning models in creative ways.


## Data and Model

(10 points) 

For our project we decided to use wikiart to get paintings of artists. We scraped paintings for 10 prominent African American artists. It was surprisingly difficuly to compile a dataset of paintings for some African American artists because wikiart did not have as in depth a repository for African American artists as they did for other white artists. We finally scraped 20 paintings for each of the following artists: 
1) Jacob Lawrence
2) Aaron Doughlas
3) Clementine Hunter
4) Jean-Michel Basquiat
5) Kerry James Marshall
6) Romare Bearden
7) Alma Woodsey Thomas
8) David Hammons
9) Henry-Ossawa-Tanner
10) William-H-Johnson

We had to ensure that all images scraped were of the same size and format in order to create our training set. 









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

There are large ethical concerns with our project. This is a current and sensitive topic to people all around the world. 

- In what future directions could you expand this work?

In the future we would like to include more African American artists paintings to create generative art and more paintings per artist. Further, we would like to represent other less represented communities in the generative arts field as well like Hispanic and LatinX artist. Further, it would be interesting to include different forms of art like scultures and other digital art, rather than just oil paintings from wikiart. This will make our dataset more diverse and allow us to generate better images. 
Further, we would like to analyse trends we see in the generative art of African American artists and see if those similar trends exist in White artists. It will be interesting to see if white artists have similar trends in their artwork, but are better represented in museums etc. 

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
https://hyperallergic.com/501999/artists-in-18-major-us-museums-are-85-white-and-87-male-study-says/