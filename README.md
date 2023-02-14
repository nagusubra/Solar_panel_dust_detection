# Solar_panel_dust_detection

## Problem Statement 

Photovoltaic systems are being adopted as an important and sustainable source of energy. Solar panels are exposed to the sun which produces electrical power. However, a common issue is dust/debris being collected on these panels which block the sun’s rays from contacting the solar cells, and in turn: reduce the energy output of the solar cells. This project's aim is to design a Convolutional Neural Network (CNN) model to detect whether a solar panel is dusty (dirty) or clean. We will also consider that this model would run on a drone and therefore will attempt to miniaturize the model while retaining meaningful performance. To guide us we will follow the findings of a research paper [1] that conceptually tackled the same problem, excluding model compression. 

## Dataset 

The selected Dataset is: Solar Panel dataset ​[2]​. This dataset contains images of solar panels collected from various regions in Bangladesh. The initial binary classification was decided to be clean and dirty. 

## Proposed Machine Learning Methods 

We will be splitting the project into 2 phases, phase 1 uses a traditional CNN to classify the images. Once the phase 1 base model performs sufficiently according to our performance metrics, the next phase would focus on model compression. Model compression will reduce the model size so that it can run on drones for solar panel inspection. The model compression techniques include but are not limited to pruning, quantization, and data augmentation. 

## Performance Metrics 

We will use accuracy to evaluate the performance of how well the model can identify whether a solar panel is dirty or clean. We are creating a model which will run on an inspection drone, hence the model must be small enough to run on the reduced hardware capabilities, while still providing accurate results. The performance metrics are model size, accuracy, loss, and inference time. 

## Expected Analysis and Trade-offs 

The expected analysis: 

The model can classify a given set of images as clean or dirty. 

Evaluation using accuracy vs model size graph, inference time vs model size graph, etc.  

The new model should be lower in size and have acceptable accuracy. 

The trade-offs for the new model: 

| Advantages | Disadvatages |
|       --- |       --- |
|Reduction in model size. | Reduction in overall accuracy. |
|Reduction in inference time. | Increase in model loss. |

## Potential Challenges 

The main challenge we expect to face is to maintain the performance of the model while we compress it to a feasible size. The research paper will provide us with a good guideline to create a good model, but it does not consider the concept of model compression which is crucial for our application. 

## References 

[1] M. S. H. Onim et al., “SolNet: A Convolutional Neural Network for Detecting Dust on Solar Panels,” 

Energies, vol. 16, no. 1, p. 155, Dec. 2022, doi: https://doi.org/10.3390/en16010155. 

[2] "Solar Dataset," [Online]. Accessed: Feb. 11, 2023. [Online]. Available: 

https://drive.google.com/drive/folders/12Q3MBI8SPw0vHsO_kkS5izkxw0F7tXx4 
