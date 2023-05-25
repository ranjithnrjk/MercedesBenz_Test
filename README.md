# MercedesBenz_Test


<h1>Business Problem</h1>

---

<h2>Description</h2>
<p>source:<a href:https://www.kaggle.com/c/mercedes-benz-greener-manufacturing>MercedesBenzGreenerManufacturing</a> </p>
<p><b>Problem statement</b>: Develop machine learning models to predict the testing time required for each custom-made Mercedes Benz car using their robust testing system. By leveraging these models, gain valuable insights and optimize the entire testing process for enhanced efficiency.</p>
<p>
Since the first automobile, the Benz Patent Motor Car in 1886, Mercedes-Benz has stood for important automotive innovations. These include, for example, the passenger safety cell with crumple zone, the airbag and intelligent assistance systems. Mercedes-Benz applies for nearly 2000 patents per year, making the brand the European leader among premium car makers. Daimler’s Mercedes-Benz cars are leaders in the premium car industry. With a huge selection of features and options, customers can choose the customized Mercedes-Benz of their dreams.
<br>
</p>
<p>
To ensure the safety and reliability of each unique car configuration before they hit the road, Daimler’s engineers have developed a robust testing system. But, optimizing the speed of their testing system for so many possible feature combinations is complex and time-consuming without a powerful algorithmic approach. As one of the world’s biggest manufacturers of premium cars, safety and efficiency are paramount on Daimler’s production lines.
<br>
</p>
<p>
In this competition, Daimler is challenging Kagglers to tackle the curse of dimensionality and reduce the time that cars spend on the test bench. Competitors will work with a dataset representing different permutations of Mercedes-Benz car features to predict the time it takes to pass testing. Winning algorithms will contribute to speedier testing, resulting in lower carbon dioxide emissions without reducing Daimler’s standards.
</p>
<br>
<h1>Mapping business problem to machine learning problem</h1>
<h2>Existing approaches</h2>
- <a href:https://www.youtube.com/watch?v=0qHXNeuNOAE>Winners talk about the problem.</a><br>
- <a href:https://www.kaggle.com/c/mercedes-benz-greener-manufacturing/discussion/36242#202443:~:text=The%2011th%20place%20solution>Winners solution.</a><br>
- <a href:https://www.kaggle.com/code/sudalairajkumar/simple-exploration-notebook-mercedes>Most Upvoted solution.</a><br>
- <a href:https://blog.goodaudience.com/stacking-ml-algorithm-for-mercedes-benz-greener-manufacturing-competition-5600762186ae>Solved using deep learning model and stacking classifier.</a>
<br>
<h2>Performance metric</h2>
- Co-efficient of determination
<br><h2>Business Constraints</h2>

- No latency requirement
- Regression problem
- Maximize R2 coefficient
- Reduce the curse of dimensionality and reduce the impact of outliers.<br>

<h2>Data overview</h2>
<p>The dataset contains two csv file</p>

- train.csv
- test.csv
    
<p>The significant observation here is that both of these files are of same size i.e, if cross validation is performed using folds. The score form one fold would be same as the 
public score in the competition. The outliers would also be more and new that the model must face apart from training set.
<br>
The traing dataset contains:</p>

- 4209 data points
- 377 features
    - Categorical features: 8
    - Constant features: 12 
    - Binary features: 356
- One target variable
