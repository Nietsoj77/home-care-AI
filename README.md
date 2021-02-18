<!-- This is the markdown template for the final project of the Building AI course, 
created by Reaktor Innovations and University of Helsinki. 
Copy the template, paste it to your GitHub README and edit! -->

# Home care AI

This is the final project for the Building AI course from <a href="https://www.elementsofai.com/">Elements of AI</a>. Please note that this is an idea for a project and not a finished solution.

## Summary

Using methods of machine learning, this project aims to identify how the required time in home care for the eldersly can be estimated from various factors that are recorded during assessment. Because of the large number of factors involved, the number of potential dependencies are too many to be handled through simple methods based on checklists or manuals.


## Background

Home care for the elderly (Swe: <i>hemtjänst</i>) in Sweden is a service provided by the municipal social services. Based on their needs, a person can be granted a number of different services. And for each service, a certain number of hours (and frequency) is allocated. Thus, the total time allocated for a person becomes a simple linear combination. Possible effects of interactions between services are usually not taken into account.

The problem arises when a person is granted several different services; the time that is <i>actually</i> required may differ from the allocated time.  which makes planning difficult. 

There are many factors that can potentially cause these differences, and the number of combinations and relationships is too large for any human to investigate. This is where AI comes in. 

## How is it used?

The project will make use of various sources of information. The main (dependent) variable will be the recorded number of hours of performed service per customer. This will be related to a number of different factors; background variables about the customers, type of services granted, and health assessment (ICF).

The input variables will be used for predicting the output, i.e. the required number of customer hours. Depending on the complexity of the resulting model, this will be done in the form of a spreadsheet or an app with a graphical user interface. 

ICF = International Classification of Functioning, Disability and Health, https://www.who.int/docs/default-source/classification/icf/icfbeginnersguide.pdf?sfvrsn=eead63d3_4


## Data sources and AI methods
The data is collected as a part of the assessment process.

As a first step, a pilot study will be done, where the relationships between the various factors will be investigated. Some models that may be applicable are:

* Linear regression
* Dimensionality reduction (PCA)
* Cluster analysis
* Support vector machine
* Neural network

The pilot study will result in a preliminary algorithm design, which will then be tested with a larger dataset. Presumably, the final model will be the result of several iterations and trials.

## Challenges

This project will hopefully improve the precision of time estimates in home care for the elderly. This, in turn, will facilitate the planning of customer visits and personnel resources. Ultimately, this will result in lower cost and higher efficiency throughout the process. As home care is a public service, this will be beneficial to the entire municipality and its citizens.

The data involved in the project describes intimate details about people's health and their need for support. It is therefore important to request permissions from the customers and to handle the data confidentially.  

## What next?

There are 290 municipalities in Sweden, and all of them are subject to the same legislation and regulations concerning home care. If the project is successful, the model can be distributed to other municipalities. If this is the case, integration with other IT-systems and automation may be relevant. But that is outside the scope of the initial project.
