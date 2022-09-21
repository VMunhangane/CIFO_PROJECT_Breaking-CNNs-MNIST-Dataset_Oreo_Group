# Computational Intelligence for Optimization (CIFO) Project: Breaking CNNs 
### Case study:MNIST-Dataset

## Introduction


On deep neural networks the convolutional neural network (CNN) has become the state-of-the-art method for image recognition. However, this method is sensitive to small perturbations, meaning that they can be easily fooled by adversarial attacks and classify images incorrectly. On this project it is going to be shown the effect of Genetic Algorithm (GA) by creating adversarial images. These images are going to be created using MNIST dataset. The test dataset is going to be evolved using the main operators of GA and the goal is to make CNN model classify images incorrectly. 

## Link to acess the project
https://github.com/VMunhangane/CIFO_PROJECT_Breaking-CNNs-MNIST-Dataset_Oreo_Group/blob/main/Report_Breaking%20CNNs%20%E2%80%93%20MNIST%20Dataset_Oreo_Group.pdf
The report is organized as follows. Section 2 shows the GA Operators, the fitness function and the constants used in this project. Section 3 describes the results of our experiments. On Section 4 and 5 are presented the conclusions and the propose for future work respectively.

## Link to acess the Notebook and others
https://github.com/VMunhangane/CIFO_PROJECT_Breaking-CNNs-MNIST-Dataset_Oreo_Group/blob/main/Breaking%20CNNs%20%E2%80%93%20MNIST%20Dataset_Oreo_Group.zip

## Some results and visualisations

#### MNIST-Dataset image 



The figure 1 provides the performance of the trained model in each label. In general, the model is well trained since it is able to predict correctly all the labels (0-9). The accuracy of the precision, recall and f1 score are 0.95%. On the following results it is going to be analyzed the performance of this model on the adversarial images.


# image of the model


The well-trained model was used to classify the adversarial images resulted from each combination of the operators. The performance of the model on each of the 12 scenarios was analysed using the classification report and plotting the accuracy, precision, recall and f1-score on each generation.


##### Fitness on each scenario
After analysing the performance of the model on each scenario evolved by the GA’s operators, was compared, the distribution of the fitness throughout 10 generations. The figure below contains thirteen box plots for each scenario.
Combining the results presented on each scenario with these box plots they clearly show that the scenarios with higher values of fitness are the ones with more adversarial images. These scenarios are able to misclassify the model. with this we can conclude that some operators succeed to maximize the fitness values throughout the 10 generations.

#### Image 

### GA operator’s
###### FPS_SPC_SM: Fitness proportion selection, single point crossover and swap mutation;
###### FPS_SPC_IM: Fitness proportion selection, single point crossover and inversion mutation;
###### FPS_AC_SM: Fitness proportion selection, arithmetic crossover, and swap mutation;
###### FPS_AC_IM: Fitness proportion selection, arithmetic crossover, and inversion mutation;
###### TS_SPC_SM: Tournament selection, single point crossover and swap mutation;
###### TS_SPC_IM: Tournament selection, single point crossover and inversion mutation;
###### TS_AC_SM: Tournament selection, arithmetic crossover, and swap mutation;
###### TS_AC_IM: Tournament selection, arithmetic crossover, and inversion mutation;
###### RS_SPC_SM: Raking selection, single point crossover and swap mutation;
###### RS_SPC_IM: Raking selection, single point crossover and inversion mutation;
###### RS_AC_SM: Raking selection, arithmetic crossover, and swap mutation;
###### RS_AC_IM: Raking selection, arithmetic crossover, and inversion mutation;
###### FPS_AC_SM_Elitism: Fitness proportion selection, arithmetic crossover, and swap mutation with elitism.

### Conclusions
After all the analysis it is clear that GA’s operators are able to create adversarial images able to make a one well trained model misclassify. we can conclude that the implementation of the GA’s operators on MNIST dataset was achieved and the main outcomes of this implementation are:
###### In general, for the constants chosen on this project the evolving using FPS got many images able to misclassify the model;
###### Some combinations of operators like TS_SPC_SM, RS_AC_SM need more generations or increasing the probability of crossover and mutation to create images able to misclassify the model;
###### The elitism did not have much impact on the fitness due to the number of the generations meaning that the evolving process only kept 10 best individuals among 1000.

### image


## Group Name: Oreo
![Happyimage png](https://user-images.githubusercontent.com/71514679/120045432-e38e7400-c007-11eb-9e44-3c655f1a967f.jpg)

### Members:  
###### Geraldo Timbe (M20200603); 
###### Manuel Carreiras(M20200603); 
###### Venâncio Munhangane (M20200579).
