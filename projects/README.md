# M2POC Projects Guidline

## Github Procedure
- Fork this github repository to your own account
- Add a folder under m2poc2019/projects, name it with your last name
- Work out your project codes/documentation and stage/push it to your folder
- Once finalised, create a pull request to the main branch

## Evaluation
You will be evaluated against the quality (description & objectives) and degree of achievement of your project.
You are expected to present your work during a 15 mins presentation at the end of the class.

Your project repository folder will need to contain at least:
- a readme file with the description of your objectives, dataset used and methods applied
- at least one jupyter notebook showcasing your methodology

## Available Dataset

This a list of possible dataset to be used in your project. With these, you can address many different scientific 
questions and demonstrate your ability to implement data mining and machine learning standard methods.

*To be updated soon*

## Suggestions

You are encouraged to seek out for your own ideas and propositions for your project.
Here is a list of possible projects to be conducted during the 2 days. 

### Clustering or unsupervised classification

- Of ocean vertical profiles. Here you can investigate the internal ocean structure of water masses and there variability.
 One can follow the Maze et al (2017) procedure [http://dx.doi.org/10.1016/j.pocean.2016.12.008] and apply it with other explanatory variables and space/time domains.
 
- Of model ensemble of vertical profiles. Look for non-gaussians signals in the intrinsic ocean variability.  

- Of atmospheric air-sea fluxes. Investigate how atmospheric weather regimes force the ocean. One can follow the 
Barrier et al (2012) procedure [http://dx.doi.org/10.1007/s00382-012-1578-7].

### Supervised classification

- Prediction of Argo Quality Control outcomes. Improve the quality control procedure of Argo data with machine learning.
One can follow the Maze et al (2018) procedure and improve it [http://www.argo.ucsd.edu/ADMT18_MachineLearning.pdf].
- Eddy detection algorithm. Building on existing datasets, use and test other classifiers.

### Regression

- Salinity against Temperature. It is crucial to be able to predict salinity using only temperature data in order to investigate the climatic signals of the upper ocean. 
- In-situ Temperature against Altimetry. Another challenge is to be able to combine satellite with in-situ data to reconstruct high-resolution 3D datasets of the ocean state.