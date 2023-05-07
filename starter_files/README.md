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
- upload a dataset; image of uploaded dataset ![image](https://user-images.githubusercontent.com/105419001/236661737-4ba96dea-d15d-4a0d-8b51-5f3fc7b565fb.png)
- create an experiment;
- configure cumpute cluster;
- run the experiment with an application insight enabled; image of completed experiment ![image](https://user-images.githubusercontent.com/105419001/236661830-0c904b7b-410e-4207-8048-fa51cf11270f.png)
- explore the best model result;image of best model summary ![image](https://user-images.githubusercontent.com/105419001/236661940-b9b14f5e-206f-4d25-853f-2d271096e6fc.png)

step 2: Deploy best model
- Click "deploy" of the best model datail tab;
- Run "logs.py" to enable application insigts; image of the insgihts is enabled![image](https://user-images.githubusercontent.com/105419001/236660532-6514318f-483b-423a-94b1-43fc5ca587c1.png) image of log bu runnning logs.py ![image](https://user-images.githubusercontent.com/105419001/236662013-dd761c53-9671-4201-b5ba-9b7efd82ba95.png)

step 3: Consume deployed model
3-1: Swagger
- download swagger.json
- run swagger.sh and surve.py
- interactive with Swagger; image of responce in Swagger TBD
3-2: Requests.post method
-
Python SDK(aml-pipelines-with-automated-machine-learning-step.jpynb)
step 1: Create automl step and pipeline
- define automl_steps
- define output
step 2: Run the pipeline
step 3: Retrieve the Best Model
step 4: Test the model; image of result
step 5: Publish pipeline
step 6: Run the pipeline from its REST endpoint


## Screen Recording
*TODO* Provide a link to a screen recording of the project in action. Remember that the screencast should demonstrate:

## Standout Suggestions
*TODO (Optional):* This is where you can provide information about any standout suggestions that you have attempted.
