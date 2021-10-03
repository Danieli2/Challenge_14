# Challenge_14

**Background**
In this Challenge, I assume the role of a financial advisor at one of the top five financial advisory firms in the world. My firm constantly competes with the other major firms to manage and automatically trade assets in a highly dynamic environment. In recent years, my firm has heavily profited by using computer algorithms that can buy and sell faster than human traders.

The speed of these transactions gave my firm a competitive advantage early on. But, people still need to specifically program these systems, which limits their ability to adapt to new data. I plan to improve the existing algorithmic trading systems and maintain the firm’s competitive advantage in the market. To do so, I enhanced the existing trading signals with machine learning algorithms that can be adapted to new data.

***

**Establish a Baseline Performance**
 The Baseline Performance of the of the of the first SVM modeling is realativly close to the actual returns with a following short window of 4 and a long window of 100. This is using svm modeling that allows me to predict with a precision of for every -1 43% of the time and a percision 56% of the time for a 1. The recall for a positive one is 94% and the recall for a negative one is 4% at the baseline model. The acuracy hovers around 50% depending on if you are looking at the macro average or weighted average.   

<img width="615" alt="Screen Shot 2021-10-02 at 7 12 08 PM" src="https://user-images.githubusercontent.com/85910138/135737041-b9508252-a5e2-4999-a3a0-76c1016fda40.png">

***

**Tune the Baseline Trading Algorithm**
I tuned the base line SVM model by extending the number of the short window to 7 and the long window to 200. This resulted in the a greater deviation of the strategy prediction returns compared with the actual returns. However, there was an increase in the percision and recall of the model by extending out the windows. The most notabel improvement is an in crease of the rcal for negative one from 4% to 14%.

<img width="622" alt="Screen Shot 2021-10-02 at 7 27 26 PM" src="https://user-images.githubusercontent.com/85910138/135737287-f0d69c5b-c180-494b-a2d2-d67b7acb1f02.png">

***

**Evaluate a New Machine Learning Classifier**
In this new machine learning model I used a logistic regression model to see if I would get better predictive powerr from the data using this specific model. Using this model I did get improved scores on the clssification report with a percision of 44% for negative one and 56% for positive one. A recall of 33% for negative one and 66% for a postive one. These results are better than the base line model which was originally used on the data. This increased recall and percison allowed for a higher accuracy of predictins than the baseline model. 

<img width="616" alt="Screen Shot 2021-10-02 at 7 37 52 PM" src="https://user-images.githubusercontent.com/85910138/135737451-3f6298fc-5e01-4c5d-b20a-5f387e8fb4ae.png">

***

**Create an Evaluation Report**

I beleive that this new model performed better than the baseline model because of the increse in percision ,recall, and accuracy. which accompanies a change from a svm model to a logistic model.The logictical Regression model which is provided demonstrateds that you can get higher accuracy of the modelby using diffrent models that will allow for greater prediction power. For axampel the macro average accuracy of the logistic regression model is 50 % where as for the baseline model the macro accuracy is 49%. Meaning that if we adjust the windows to 7 and 200 I would propably see an improvement. However, I did not see the improvements of the prediction power of the model that I was hoping for instead it was worse as shown by the following png file.

<img width="627" alt="Screen Shot 2021-10-02 at 7 47 56 PM" src="https://user-images.githubusercontent.com/85910138/135737620-f83e40ab-4629-4343-b93b-1a258922ba61.png">

This promted me to revert back to the original model framework  for the windows to determine if I could improve it another way. The other way which I tried to improve it was by switching out the model and for a Decision tree classifier this model performed about as well as the logistic regression model but with lower accuracy. In the end I decided to stick with the logistic regression model which slightly out performed the baseline but which I belive is the best model.



