# nLpDecipher

## Overview
This project predicts the gender of a sentence that some users write. Given any sentence, the model will output male or female which represents the gender of the user who writes that sentence. We deployed a Django website for user interaction, displaying the result and related evidence in real time. We used L1/L2 norm to extract the most significant words/n-grams that determine the prediction. We also used the package Lime Text Explainer to further support the prediction based on the confidence interval of each feature.

## How to run
To run the website, first install Django and LIME.

> pip install Django
> pip install lime

Refer to the following sites for full installation instructions.
https://docs.djangoproject.com/en/2.2/topics/install/
https://github.com/marcotcr/lime

After the packages are install, inside nLpDecipher/decipher, run

>python manage.py runserver

Then use a browser to open
127.0.0.1:8000

After opening the website, click the "Train Model" button to train models.

After the "Training Done" text appears below the button, we can now input
text in either of the textbox and then click the button below to predict.

The predictions should show up shortly after one of the buttons is clicked.
