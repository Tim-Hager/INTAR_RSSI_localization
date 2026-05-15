# Where-fi - Object localization using RSSI of Wi-fi signals indoors
### INTAR Project RSSI localization
- Uses dataset UjiIndoorLoc

## Ideas:
- Autoencoder: Encoder down to dimension 3, Decoder back up, afterwards classification heads for classification/regression
- Contrastive learning: Similar to autoencoder, but without using labels

## ToDo-List:
### [x] Analysis of dataset
[x] Missing values
[x] Format
[x] Necessary data preparation
[x] Research possible augmentation
### [x] Data preprocessing
[x] Possibly transformation
[x] Data normalization
[x] Create Dataset & Dataloader -> get_dataset
[x] Split up into training-, validation- & test-set
[x] Apply augmentation
### [x] Training loop
[x] Setup training loop with optimizer and criterion (loss function)
[x] Classification & regression in one training (added to one lost-function for example or just parallel)? Might be worth a try
[x] Evaluation of model
### [ ] Model(s)
[ ] Create architecture
[ ] Define hyperparameters (use configuration), flexible architecture
[ ] Adapt training & evalation if necessary
[ ] Autoencoder with classification & regression head
[ ] Maybe contrastive learning
### [ ] Hyperparameter optimization
[ ] Simple optimization algorithm already included
[ ] Maybe Bayesian Optimization?
### [ ] Floor per building
[ ] Possibility of switching from 5 floors in general to classifyfing each building floor itself (due to height differences etc.)
[ ] Add parameter to config