This FINAL PROJECT DIRECTORY will be updated as elements of my ULTIMATE MODEL are refined and integrated.

This Final Project Directory is split into 3 folders.
1. ReferenceModels -- Contains Assignments that possibly help inform/design my FinalsModels
2. FinalModels -- Contains 2 Folders with all models and documentation for models trained and models deployed.
  --1. FinalDocumentation -- Contains Various Notebooks detail methods for refining my Models
  --2. FinalDeployable -- Contains (pkl,h5,pth,keras,etc.) files that store trained models, weights, and scalars used in the HuggingFace Deployment.
3. DataHelpers -- This folder contains the python scripts used to gather, transform, and pre-preprocess data, data sets, and data structures.
4. Datasets -- csv files structured and organized for specific tasks and needs
  


My first commit for each of the following models are trained. Subsequent commits are cleaned for legibility and integration into the final pipeline and ensemble prediction/binary recommendation model.
*THE ONLY GUARANTEED FINISH AND DEPLOYED MODEL BY THE 12/2 11:59pm due date is *Model 2*.
Models 1 will not be deployed in the ULTIMATE MODEL.
Model 3 is finished but requires Model 2 to be integrated while produce stats/data legible to this random forest predictor.

The original intention of this project was to produce a proof of concept for a Strategy Recommendation System. After several days of data processing and model training, this project has turned into an intitial reasearch survey and "____" of possible and methods and solutions to building different pieces of this project.


My models...
1. Shot Chart PNG Outcome Classifier -- Predicts a Win or Loss Given a shot chart (Image Classifier -- RNN trained on 2460 PNGs)
   ** I don't know if I will use this model... If I may simulate a shot chart/selection given a each player's shot profile
   -- I can easily train a similar model that looks at shot distance histograms or a tabular equivalent.
2. Stat Line Predictor (by Previous Performances) -- Given a sequence of games from a player, what can we expect the stat line of this player to be in the next contest (LTSM)
3. PTS Predictor -- From a stat line (primarily attempted shots) can we predict a Player's point total in that contest (Random Forest)
4. Predict Game Outcome Given a Team's stat line (Previously Trained Neural Net)

Final Ensemble Flow -- Model 2 Feeds Model 3 for Team Players --> Stats Aggregated to Feed Model 4 --> Determine if Strategic Intervention is Required
Model 2 (All Players of Selected Team) --> Stats Predictions --> Points Prediction ] VERIFY? --> 
                                       --    --   --   --    --> Points Prediction ]
