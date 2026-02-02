# CNN - German Traffic Sign Detection (GTSDB)
## OBJECTIVE
Implement a Convolutional Neural Network (CNN) to detect and classify German traffic signs using the GTSDB dataset.

## TO-DO LIST
- Try data augmentation techniques.
- Try data augmentation with brightness/contrast and rotation.

## JOURNAL
### 01-02-2026
- Analyzed the discrepancy between actual and prediction values in test dataset evaluation.
- Increased EPOCHS from 20 to 100. Observed overfitting signs. Try early stopping, increase dropout and data augmentation.

### 18-12-2025
- Added initial notebook configurations, structure and code.
- Decisions made:
    - From Detection to Classification: Although the original dataset is for detection (finding the sign in the large photo), I decided to crop the signs. This allows me to focus on a pure classification model, which is more simple and educational as a first step.
    - Change of Granularity (Types vs. Classes): The dataset has 43 specific classes, but some had only 1 sample, making it impossible for the model to learn (causing stratification errors). I decided to group the 43 classes into 5 functional categories: Prohibition, Danger, Mandatory, Priority / Stop, End of Restriction.