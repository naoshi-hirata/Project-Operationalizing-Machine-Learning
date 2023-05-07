*NOTE:* This file is a template that you can use to create the README for your project. The *TODO* comments below will highlight the information you should be sure to include.


# TITLE: "Building a Machine Learning Model and Creating a Pipeline for the Bank Marketing Dataset Using Azure"

*TODO:* Write an overview to your project.
# The purpose of this project is to use Azure to build a machine learning production model and create and use a pipeline.

## Architectural Diagram
*TODO*: Provide an architectual diagram of the project and give an introduction of each step. An architectural diagram is an image that helps visualize the flow of operations from start to finish. In this case, it has to be related to the completed project, with its various stages that are critical to the overall flow. For example, one stage for managing models could be "using Automated ML to determine the best model". 
![azureMLstudio_architecture](https://user-images.githubusercontent.com/105419001/236659616-b4e0904b-99ef-4b22-b344-982f6d633798.png)
![pipeline_architecture](https://user-images.githubusercontent.com/105419001/236659624-b46f1255-4283-4e68-b8df-5b8b75b818f6.png)



## Key Steps
*TODO*: Write a short discription of the key steps. Remeber to include all the screenshots required to demonstrate key steps. 
AutoML studio
step 1: Create an experiment using Automated ML
- upload a dataset; 
- create an experiment;
- configure cumpute cluster;
- run the experiment
step 2: Deploy best model
step 3: Consume deployed model
3-1: Swagger
-
3-2: Requests.post method
-
Python SDK(aml-pipelines-with-automated-machine-learning-step.jpynb)
step 1: Create automl step and pipeline
- define automl_steps
- define output
step 2: Run the pipeline
step 3: Retrieve the Best Model
step 4: Test the model
step 5: Publish pipeline
step 6: Run the pipeline from its REST endpoint

## Screen Recording
*TODO* Provide a link to a screen recording of the project in action. Remember that the screencast should demonstrate:

## Standout Suggestions
*TODO (Optional):* This is where you can provide information about any standout suggestions that you have attempted.
