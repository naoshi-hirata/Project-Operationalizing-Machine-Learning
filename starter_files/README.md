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
- interactive with Swagger; image of responce in Swagger ![image](https://user-images.githubusercontent.com/105419001/236768792-64a1f158-1aa1-4af3-b53f-4fcc33759f12.png)
3-2: Requests.post method
-
Python SDK(aml-pipelines-with-automated-machine-learning-step.jpynb)
step 1: Create automl step and pipeline
- define automl_config
- define outputs
- create pipeline
step 2: Run the pipeline
step 3: Retrieve the Best Model
step 4: Test the model using test dataset; image of result ![image](https://user-images.githubusercontent.com/105419001/236662196-bb6a67e7-9212-473d-a6ce-d7a390385c38.png), image of request ![image](https://user-images.githubusercontent.com/105419001/236662247-af3aab0d-8085-4140-8800-df824ddb6482.png)

step 5: Publish pipeline; image of created pipeline ![image](https://user-images.githubusercontent.com/105419001/236662290-ea2f9c8f-79d4-41e9-867f-d8e2337d13dc.png),image of pipeline endpoint ![image](https://user-images.githubusercontent.com/105419001/236662356-5f083023-6012-4ee8-a566-7c71137ddb85.png), image of pipeline ![image](https://user-images.githubusercontent.com/105419001/236662412-6d215112-cd14-4df8-9db3-2910b799cee4.png), image of publishe pipeline overview ![image](https://user-images.githubusercontent.com/105419001/236662463-9dc61376-395d-4c5e-9e37-1d00d06cc824.png)

step 6: Run the pipeline from its REST endpoint; image of result ![image](https://user-images.githubusercontent.com/105419001/236662548-4ddb2e44-1981-49ac-8ba9-0be89162c954.png), image of scheduled running ![image](https://user-images.githubusercontent.com/105419001/236662598-4102ca56-e110-42ad-8797-efa866d0bb6d.png)

## Screen Recording
*TODO* Provide a link to a screen recording of the project in action. Remember that the screencast should demonstrate:https://github.com/naoshi-hirata/Project-Operationalizing-Machine-Learning/blob/master/sample_screenshots/Building%20a%20Machine%20Learning%20Model%20and%20Creating%20a%20Pipeline%20for%20the%20Bank%20Marketing%20Dataset%20Using%20Azure.mp4

## Standout Suggestionsrun result
*TODO (Optional):* This is where you can provide information about any standout suggestions that you have attempted.
