# Analysis results
## Dataset general information
- 529 Attributes
    - 1 - 520: Intensity values of WLAN signals
        - -104...+100 --> Easy normalization
        - Value of +100 means not detected
    - 521 & 522: Longitude & Latitude --> Label for regression
        - Specific min/max values --> Easy normalization
    - 523: Altitude in form of floors of the building --> Label for regression (but discrete values? --> Afterwards rounding (before loss))
        - 0...4 --> Easy normalization
    - 524 & 525: Building & Space ID --> Labels for classification
    - 526 - 529: Irrelevant
- Training set & validation set given by different CSV-files
    - Validation set recorded later
        - Different localization of room decor etc --> Much more difficult
        - Perfect for test set
    - Validation set is only 5% of all data, but with 1.111 samples easily big enough
    - Split training set into 90% training and 10% validation set for hyperparameter training
        - Important: Statistical same distribution of each Space & Building!!!

## Dataset analysis
- No NaN values
- Duplicate rows in training data --> Remove!
