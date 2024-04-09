# deep-learning-challenge
REPORT on the Neural Network Model for Alphabet Soup

Overview of the Analysis:

The purpose of this analysis is to develop a deep learning model using a neural network to predict the success of funding applicants for Alphabet Soup, a philanthropic organization. By utilizing historical data provided by Alphabet Soup, the aim is to create a model that accurately classifies applicants as successful or unsuccessful based on various features.

Results:

Data Preprocessing:

Target Variable: The target variable for the model is IS_SUCCESSFUL, indicating whether an applicant was successful (1) or unsuccessful (0).
Features: Features include columns such as APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT, among others.
Variables Removed: Non-beneficial ID columns (EIN and NAME), as well as STATUS, SPECIAL_CONSIDERATIONS, and ASK_AMT, were removed as they are neither targets nor features.
Compiling, Training, and Evaluating the Model:

Attempt #1:

Architecture: Two hidden layers with 80 and 30 neurons, respectively, both using ReLU activation functions.
Performance: Loss: 0.56, Accuracy: 72.98%.
Observation: Model accuracy falls short of the target of 75%.

Attempt #2:

Changes Made: Dropped non-beneficial columns and replaced low-frequency categories in APPLICATION_TYPE and CLASSIFICATION.
Architecture: Added a third hidden layer with 10 neurons, all using ReLU activation functions.
Performance: Loss: 0.5667, Accuracy: 72.84%.
Observation: Accuracy did not improve significantly from Attempt #1.

Attempt #3:
Changes Made: Changed activation functions to tanh in the second and third hidden layers.
Architecture: Kept the same architecture as Attempt #1.
Performance: Loss: 0.5578, Accuracy: 73.08%.
Observation: Slight improvement in accuracy achieved.
Summary:

The deep learning model's performance did not meet the target accuracy of 75% in any attempt. Despite making adjustments to the model architecture and data preprocessing, the desired performance was not achieved. Further experimentation may be necessary, such as exploring different model architectures, tuning hyperparameters, or incorporating additional features.

A recommendation for a different approach to solving this classification problem would be to explore ensemble learning methods, such as Random Forest, which may provide better predictive performance compared to a single neural network model. Additionally, using techniques like feature engineering or applying more sophisticated preprocessing methods could potentially improve model performance. Experimentation with various models and techniques is crucial to finding the most effective solution for the problem at hand.





