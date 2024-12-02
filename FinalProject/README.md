This will turn into some combination of proposal and documentation/write-up. . . I think. If this works.


My models...
1. Shot Chart PNG Outcome Classifier -- Predicts a Win or Loss Given a shot chart (Image Classifier -- RNN trained on 2460 PNGs)
   ** I don't know if I will use this model... If I may simulate a shot chart/selection given a each player's shot profile
   -- I can easily train a similar model that looks at shot distance histograms or a tabular equivalent.
3. Stat Line Predictor (by Previous Performances) -- Given a sequence of games from a player, what can we expect the stat line of this player to be in the next contest (LTSM)
4. PTS Predictor -- From a stat line (primarily attempted shots) can we predict a Player's point total in that contest (Random Forest)
5. Predict Game Outcome Given a Team's stat line (Previously Trained Neural Net)

Ensemble Flow -- Model 2 Feeds Model 3 for Team Players --> Stats Aggregated to Feed Model 4 --> Determine if Strategic Intervention is Required
Model 2 (All Players of Selected Team) --> Stats Predictions --> Points Prediction ] VERIFY? --> 
                                       --    --   --   --    --> Points Prediction ]
