# multilinear.regression_assignment
this is my multi linear regression model training assignment.

I was stuck on one Machine Learning assignment for 4 days… and I'm actually glad I didn't give up.
When I first started building a Multiple Linear Regression model, I thought the hardest part would be writing the code.
I was wrong.
The real challenge was understanding which features actually matter and why the model predicts what it predicts.
For the last 4 days, I kept testing, failing, asking questions, and experimenting until everything finally started making sense.
🎯 My goal
Predict the Adulteration Percentage in fuel using Multiple Linear Regression.
But instead of training just one model, I decided to experiment.
🔬 Experiment 1
Initially, I trained my model using only three features:
✔️ Density
✔️ Viscosity
✔️ Adulterant Type
The result?
📉 R² Score = 0.591
That was my biggest learning moment.
Although these are the most important fuel properties, they were not enough to explain the adulteration percentage accurately.
So instead of accepting the result, I asked myself:
What if the model needs more useful information?
🔬 Experiment 2
I included additional fuel properties along with Density, Viscosity, and Adulterant Type.
The improvement was immediately visible.
📈 R² Score improved from 0.591 ➜ 0.761
That single experiment completely changed the way I think about Machine Learning.
💡 Biggest Lesson
I used to believe:
"The more features you use, the better the model becomes."
Now I know the reality is different.
✔️ Sometimes too few features are not enough.
✔️ Sometimes adding relevant features improves the model significantly.
✔️ But adding irrelevant features can also hurt performance.
Machine Learning isn't about using more data.
It's about using the right data.
🛠 Things I learned while building this project
✅ Handling missing values
✅ Feature Selection
✅ Encoding categorical data using pd.get_dummies()
✅ Understanding why drop_first=True is used
✅ Building the Feature Matrix (X) and Target (y)
✅ Training the model
✅ Making predictions
✅ Understanding coefficients and intercept
✅ Manually verifying predictions instead of blindly trusting the model
✅ Evaluating performance using:
R² Score
MAE
MSE
✅ Creating an Actual vs Predicted visualization to understand model behavior.
📊 Final Model Performance
📈 R² Score: 0.7611
📉 MAE: 4.43
📉 RMSE: 7.13
The model isn't perfect—and that's okay.
What matters most is that I now understand how to evaluate a regression model instead of only checking whether the code runs.
🔹 I learned that a regression model cannot understand string (categorical) values directly.
For example, my dataset contained an Adulterant column with values like:
Ethanol
Kerosene
Methanol
None
Before training the model, I converted these categorical values into numerical features using pd.get_dummies().After encoding the categorical data,
I used pd.concat() to combine the newly created dummy columns with my numerical features, creating the final feature matrix for the model.
This assignment helped me realize that data preprocessing is just as important as model building.
🌱 Final Thought
Coming from a non-technical background, there are days when a single assignment takes me four days to finish.
But every bug, every failed experiment, and every question teaches me something that a copied solution never could.
This assignment wasn't just about Multiple Linear Regression.
It was about learning how to think like a Machine Learning practitioner.
two experiment.
multiples mistake.
multiples lesson at a time.
