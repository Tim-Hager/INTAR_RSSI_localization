# Where-fi - Object localization using RSSI of Wi-fi signals indoors
### INTAR Project RSSI localization
- Uses dataset UjiIndoorLoc

## Ideas:
- Autoencoder: Encoder down to dimension 3, Decoder back up, afterwards classification heads for classification/regression
- Contrastive learning: Similar to autoencoder, but without using labels

## ToDo-List:
### [ ] Analysis of dataset
[ ] Missing values
[ ] Format
[ ] Necessary data preparation
[ ] Research possible augmentation
### [ ] Data preprocessing
[ ] Possibly transformation
[ ] Data normalization
[ ] Create Dataset & Dataloader -> get_dataset
[ ] Split up into training-, validation- & test-set
[ ] Apply augmentation
### [ ] Training loop
[ ] Setup training loop with optimizer and criterion (loss function)
[ ] Classification & regression in one training (added to one lost-function for example or just parallel)? Might be worth a try
[ ] Evaluation of model
### [ ] Model(s)
[ ] Create architecture
[ ] Define hyperparameters (use configuration), flexible architecture
[ ] Adapt training if necessary
[ ] Autoencoder with classification & regression head
[ ] Maybe contrastive learning
### [ ] Hyperparameter optimization
[ ] Simple optimization algorithm already included
[ ] Maybe Bayesian Optimization?