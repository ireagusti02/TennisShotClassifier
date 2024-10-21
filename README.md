# TennisShotClassifier

The aim of this project was to utilize deep learning to classify types of tennis shots as early and accurately as possible from labeled video data. Due to a lack of access to the required computational resources and overloading of the accessible RAM, the project shifted to an image classification task, where we built a CNN using PyTorch. We acknowledge two major flaws in this classification task: first, we had to manually label the shots based on our perception as varsity tennis players (as early as possible), which could introduce inconsistency; second, by ignoring the temporal aspect, we ended up classifying different stages of a tennis shot as the same, making the task more challenging.

### In this repository, you will find:

*Data*: 
- `game1` and `game8` folders contain individual clip classifications. 
- The `images` folder contains the raw image data. 

*Processing*: 
- `game1.csv` and `game8.csv` combine the clip information into a single data frame. 
- `game18_2.csv` combines the data frames from `game1` and `game2`. 
- `game182_fixed.csv` manually addresses an issue with missing data. 
- The `images2` folder contains renamed, resized, and recolored images. 

*Code*: 
- `DataPrep.ipynb` contains data processing scripts. 
- `Models.ipynb` contains the CNN model. 
- `3Dcnn.ipynb` contains an attempt at a 3D CNN model. 

### Next steps
This project was cut short due to time constraints. Having worked with time-series data since then, I have identified some sources of inefficiency. We could benefit from using built-in deep learning time-series models such as InceptionTime to return to the original objective of the project.


