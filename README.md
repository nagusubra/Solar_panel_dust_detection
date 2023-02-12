# Solar_panel_dust_detection

## Problem Statement 

Photovoltaic systems are being adopted as an important and sustainable source of energy. Solar panels are exposed to the sun which produces electrical power. However, a common issue is dust/debris being collected on these panels which block the sun’s rays from contacting the solar cells, and in turn: reduce the energy output of the solar cells. This project's aim is to design a Convolutional Neural Network (CNN) model to detect whether a solar panel is dusty (dirty) or clean. We will also consider that this model would run on a drone and therefore will attempt to miniaturize the model while retaining meaningful performance. To guide us we will follow the findings of a research paper ​[1]​ that conceptually tackled the same problem, excluding model compression. 

## Dataset 

The selected Dataset is: Solar Panel dataset ​[2]​. This dataset contains images of solar panels collected from various regions in Bangladesh. The initial binary classification was decided to be clean and dirty. 

## Proposed Machine Learning Methods 

The proposed Machine Learning (ML) model to be used in our project is a CNN model. We will be splitting the project into 2 phases, where phase 1 is to use a traditional CNN to classify the images. Once the phase 1 base model performs sufficiently according to our performance metrics, the next phase would focus on model compression. The model compression will reduce the model size so that it can run on drones for solar panel inspection. 

## Performance Metrics 

To validate the performance of our CNN model we will use accuracy to measure how well the model can identify whether a solar panel is dirty or clean. We will also evaluate the performance of our model considering the size of the model itself. We are creating a model which will run on an inspection drone, hence the model must be small enough to run on the reduced hardware capabilities, while still providing accurate results. The performance metrics are model size, accuracy, and loss. 

## Expected Analysis and Trade-offs 

The expected analysis: 

The model can classify a given set of images as clean or dirty. 

The new model should be lower in size when compared to the base model. 

The trade-offs for the new model: 

| Advantages | Disadvatages |
|       --- |       --- |
|Reduction in model size. | Reduction in overall accuracy. |
|Reduction in inference time. | Increase in model loss. |

## Potential Challenges 

The main challenge we expect to face is to maintain the performance of the model while we compress it to a feasible size. The research paper will provide us with a good guideline to create a good model, but it does not consider the concept of model compression which is crucial for our application. 
