# Neural_Network_Charity_Analysis

## Project Overview
### Purpose
I've been asked to assist Alphabet Soup in creating a binary classifier that is capable of predicting whether invesment applicants will be successful if funded by Alphabet Soup.

## Results
### Data Preprocessing
- The target variable for the model is 'IS_SUCCESSFUL' as this is a binary variable that tells us whether or not an applicant use the investment money successfully.
- The features for the model are Application Type, Affiliation, Classification, Use Case, Organization, Status, Income Amount, Special Considerations, and Ask Amount.
- The variables that are neither targets nor features are Name and EIN - I removed these variables from the model.

### Compiling, Training, and Evaluating the Model
![Initial model](https://github.com/secicciari/Neural_Network_Charity_Analysis/blob/main/Resources/initial_model.PNG)
- Initially, I built my model with one hidden layer with 100 neurons, and using the relu activation for the hidden layer and the sigmoid activation for the output layer. 
I ended up with 38 input features, so I used 100 neurons because that is roughly 3 x 38. I chose the relu activation for the hidden layer because we are concerned with identifying nonlinear characteristics from the input values.
- Unfortunately, I was not able to achieve the target model performance of 75% accuracy.
- In order to try and increase the performance of the model, I dropped additional unnecessary features (Organization and Status), I increased the number of values for each bin for both Classification and Application type, and I increased the number of neurons and added a second hidden layer. 

## Summary
In summary, both my original model and my 'optimized' model only showed about 73% accuracy when it came to predicting an investment's success. Because of the relatively low accuracy, I don't think this model would be very effective for Alphabet Soup to use.

I would recommend building an SVM to more accurately predict whether an applicant will be successful with an investment from Alphabet Soup because for straightforward binary classification problems (like we're working with here), SVMs tend to outperform neural networks and deep learning models.
