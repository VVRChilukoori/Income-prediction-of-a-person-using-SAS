<ul>
<li><b>Executive Summary</b></li>
</ul>
<p>The goal of the project is to predict what all factors makes the basis for a person to earn an income greater than $ 50K.&nbsp; In this project we will determine this by examining a data set from Census Bureau database (obtained from kaggle.com).&nbsp; We have obtained the data for the year 1994</p>
<ul>
<li><b>Business Problem/Opportunity</b></li>
</ul>
<p>In this project we consider income as a gross income earned by a person excluding taxes levied on income, social security, loan payments, medicare deductions etc. Most of the companies share their profits with employees by giving employee salaries of non-cash way such as food coupons, gift vouchers, health benefits, stock holdings etc.</p>
<p>The data is obtained from 1994 Census Bureau database. Along with the gross income of a person the bureau collects alternative income measures that can be systematically added to or removed from the income components such as deduction of taxes like state taxes and federal taxes from the payroll, including the value of specific noncash benefits like health insurance programs, food coupons, housing loans, and home equity returns. These different measures are obtained from the information gathered in Census through surveys along with the data obtained from some other agencies like the U.S. Bureau of Labor Statistics, Centers for Medicare and Medicaid Services (CMS), the U.S. Department of Agriculture, the U.S. Internal Revenue Service, and the U.S. Office of Personnel Management (OPM).</p>
<ul>
<li><b>Business Objective</b></li>
</ul>
<p>This CIS575 project proposes to determine which variables or factors, form the condition that would imply high income or low income.&nbsp; This project also proposes to identify key factors that are most decisive for determining the income of a person.</p>
<ul>
<li><b>Process for selecting and Gathering Data</b></li>
</ul>
<p>In defining the business problem and opportunity, the project team brainstormed on the relevance of a number of factors that have impacted Adult income. Team members considered their own personal experiences as well as those of the classmates, family members and friends.&nbsp; The project team also considered those factors that have been known contributors to adult income more than 50K annually including Age, workclass, education , relationship , race&nbsp; etc.</p>
<p>Preliminary discussions identified 13 variables that could contribute to student&rsquo;s persistence and graduation rates, including, but not limited to:</p>
<ul>
<ul>
<ul>
<li>Marital_status</li>
<li>Age</li>
<li>WorkClass</li>
<li>Education</li>
<li>Occupation</li>
<li>Relationship</li>
<li>Race</li>
<li>Capital_gain</li>
<li>Capital_loss</li>
<li>Hours_per_week</li>
<li>Education_num</li>
<li>Sex</li>
<li>Native_Country</li></ul></ul></ul>
<ul>
<li><b>Discussion of preliminary data exploration and findings</b></li>
</ul>
<p>SAS Enterprise Guide and Microsoft Excel were used to conduct preliminary descriptive analytics of our and to make general inferences about the variables we are considering.</p>
<p><b>List of variables and their Roles &ndash;</b></p>


<p align="center"><img src="https://github.com/VVRChilukoori/Income-prediction-of-a-person-using-SAS/blob/branch/img/1.jpg" alt="" width="776" height="489" /></p>


<p>&nbsp;</p>
<p>Variables like capital_gain, capital_loss, education_num were rejected because of their insignificant contribution towards calculation of final target variable. We have created a new column for target variable based on the income data. The target variable consists of binary values. 1 is allotted for income &gt;50K and 0 for income &lt;=50K.</p>
<p>In exploring and considering the variables for greatest relevance, the project team decided to conduct further analysis on the following variables. The variables and descriptive analysis is mentioned below:</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp; </p>
<p>&nbsp; &nbsp; &nbsp; The variables and descriptive analysis of the variable is noted below: </p>
<ul><ul><ul>
<li>Age</li>
<li>Hours_per_week</li>
<li>Fnlwgt</li>
<li>Education</li>
<li>Race</li>
<li>Relationship</li>
<li>Marital_status</li>
<li>Sex</li>
<li>Workclass</li>
<li>Occupation</li>
</ul></ul></ul>
<p>Total Number of Observations &ndash; 32561</p>

<table width="727">
<tbody>
<tr>
<td width="128">
<p><strong>Variable</strong></p>
</td>
<td width="142">
<p><strong>Descriptive Analysis</strong></p>
</td>
<td width="456">
<p><strong>Chart</strong></p>
</td>
</tr>
<tr>
<td width="128">
<p><strong>Age</strong></p>
<p>&nbsp;</p>
<p>Mean = 38.55125</p>
<p>Minimum = 17</p>
<p>Maximum = 90</p>
<p>&nbsp;</p>
<p>Std Deviation = 13.64</p>
<p>&nbsp;</p>
</td>
<td width="142">
<p>The Age in the graph appears non-normally distributed. It appears to right skewed and man is less than median.</p>
<p>&nbsp;</p>
<p><strong>X-axis</strong>: Age</p>
<p><strong>Y-axis</strong>: Frequency</p>
</td>
<td width="456">

<p align="center"><img src="https://github.com/VVRChilukoori/Income-prediction-of-a-person-using-SAS/blob/branch/img/2.jpg" alt="" width="456" height="300" /></p>

</td>
</tr>
<tr>
<td width="128">
<p><strong>Hours_per_week</strong></p>
<p>&nbsp;</p>
<p>Maximum = 99</p>
<p>Std Deviation = 12.3474</p>
<p>Mean = 40.4949</p>
<p>Minimum = 1</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
</td>
<td width="142">
<p>&nbsp; The chart for hours_per_week on the right appears to be distributed towards the center and towards the tails. It has leptokurtotic distribution.</p>
<p><strong>X-axis:</strong> hours_per_week</p>
<p><strong>Y-axis:</strong> Frequency</p>
</td>
<td width="456">

<p align="center"><img src="https://github.com/VVRChilukoori/Income-prediction-of-a-person-using-SAS/blob/branch/img/3.jpg" alt="" width="456" height="300" /></p>

</td>
</tr>
<tr>
<td width="128">
<p><strong>Fnlwgt</strong></p>
<p>&nbsp;</p>
<p>Mean = 189778.37</p>
<p>Minimum = 12285.00</p>
<p>Maximum = 1484705.0</p>
<p>Std Deviation = 105549.98</p>
<p>&nbsp;</p>
</td>
<td width="142">
<p>The chart for Fnlwgt on the right has non-normal distribution. It appears to be right skewed with mean less than median.</p>
<p><strong>X-axis</strong>: fnlwgt</p>
<p><strong>Y-axis</strong>: Frequency&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
</td>
<td width="456">

<p align="center"><img src="https://github.com/VVRChilukoori/Income-prediction-of-a-person-using-SAS/blob/branch/img/4.jpg" alt="" width="456" height="300" /></p>

</td>
</tr>
<tr>
<td width="128">
<p><strong>Education</strong></p>
<p>Hs-grad &ndash; 31.93%</p>
<p>Some college -22.6%</p>
<p>10<sup>th</sup> &ndash; 2.835%</p>
<p>Doctorate -1.24%</p>
<p>Prof-Student- 1.75%</p>
<p>Bachelors -16.825%</p>
<p>Masters-5.265%</p>
<p>11<sup>th</sup> -3.54%</p>
<p>Assoc -voc &ndash; 3.2%</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
</td>
<td width="142">
<p>31.93% of people are HS-Grad, 22.60% belong to some college.</p>
<p>&nbsp;</p>
<p><strong>X-axis</strong>: Education</p>
<p><strong>Y-axis</strong>: Frequency</p>
</td>
<td width="456">

<p align="center"><img src="https://github.com/VVRChilukoori/Income-prediction-of-a-person-using-SAS/blob/branch/img/5.jpg" alt="" width="456" height="300" /></p>

</td>
</tr>
<tr>
<td width="128">
<p><strong>Race</strong></p>

<p>White &ndash; 85.61%</p>

<p>Asian &ndash; 3.23%</p>

<p>American &ndash; 0.8%</p>

<p>Other -0.7%</p>
</td>
<td width="142">
<p>The Adult census income data for Race has majority of Whites (85.61%) and then Asians with 3.23% and rest of Americans and other Race.&nbsp;&nbsp;</p>
<p><strong>X-axis</strong>: race</p>
<p><strong>Y-axis</strong>: Frequency</p>
</td>
<td width="456">

<p align="center"><img src="https://github.com/VVRChilukoori/Income-prediction-of-a-person-using-SAS/blob/branch/img/6.jpg" alt="" width="456" height="300" /></p>

</td>
</tr>
<tr>
<td width="128">
<p><strong>Relationship</strong></p>
<p>&nbsp;</p>
<p>Not In family -25.75%</p>
<p>&nbsp;</p>
<p>Unmarried -10.365%</p>
<p>Own-child- 15.48%</p>
<p>Husband &ndash; 40.45%</p>
<p>Wife -4.89%</p>
<p>&nbsp;</p>
<p>Other-relative-3.06%</p>
<p>&nbsp;</p>
</td>
<td width="142">
<p>The data collected for variable relationship shows that among all 25.75% are Not In family, 10.365% are Unmarried, 15.48% have Own-child and 40.45% have Husband and 4.89% have Wife.</p>
<p><strong>X-axis</strong>: relationship</p>
<p><strong>Y-axis</strong>: Frequency</p>
</td>
<td width="456">

<p align="center"><img src="https://github.com/VVRChilukoori/Income-prediction-of-a-person-using-SAS/blob/branch/img/7.jpg" alt="" width="456" height="300" /></p>

</td>
</tr>
<tr>
<td width="128">
<p><strong>Marital_status</strong></p>
<p><strong>&nbsp;</strong></p>
<p>Widowed &ndash; 2.99%</p>
<p>Divorced &ndash; 13.55%</p>
<p>Separated &ndash; 3.08%</p>
<p>Never-Married-33.025%</p>
<p>Married-civ-s &ndash; 46.015%</p>
<p>Married spouse-1.24%</p>
<p>Married-AF-sp &ndash; 0.09%</p>
</td>
<td width="142">
<p>The data reveals that majority of people have status of Married-civ-s (46.0155) and 33.025% are Never married. While 13.55% are Divorced are only small percentage (2.99%) are widowed.</p>
<p><strong>X-axis</strong>: marital_status</p>
<p><strong>Y-axis</strong>: Frequency</p>
</td>
<td width="456">

<p align="center"><img src="https://github.com/VVRChilukoori/Income-prediction-of-a-person-using-SAS/blob/branch/img/8.jpg" alt="" width="456" height="300" /></p>

</td>
</tr>
<tr>
<td width="128">
<p><strong>Sex</strong></p>
<p><strong>&nbsp;</strong></p>
<p>Male &ndash; 67.185%</p>
<p>Female &ndash; 32.815%</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
</td>
<td width="142">
<p>Among the data collected 67.185% are Males and 32.815% are Females.</p>
<p>&nbsp;</p>
<p><strong>X-axis</strong>: sex</p>
<p><strong>Y-axis</strong>: percent</p>
</td>
<td width="456">

<p align="center"><img src="https://github.com/VVRChilukoori/Income-prediction-of-a-person-using-SAS/blob/branch/img/9.jpg" alt="" width="456" height="300" /></p>

</td>
</tr>
<tr>
<td width="128">
<p><strong>WorkClass</strong></p>

<p>Private -69.845%</p>
<p>Self-emp-not-inc</p>
<p>7.83%</p>
<p>Self-emp-inc 3.4%</p>
<p>Federal-gov 2.81%</p>
<p>State-gov 3.955%</p>

<p>Local-gov 6.425%</p>

</td>
<td width="142">
<p>Majority of Workclass is private with 69.845% and 2.81% are Federal-gov employee.3.955% belong to state &ndash;gov and 6.425% belong to Local-gov.</p>
<p><strong>X-axis</strong>: WorkClass</p>
<p><strong>Y-axis</strong>: Frequency</p>
</td>
<td width="456">

<p align="center"><img src="https://github.com/VVRChilukoori/Income-prediction-of-a-person-using-SAS/blob/branch/img/10.jpg" alt="" width="456" height="300" /></p>

</td>
</tr>
<tr>
<td width="128">
<p><strong>Occupation</strong></p>
<p>&nbsp;</p>
<p>Machine-op-inspct &ndash; 6.07%</p>
<p>Prof-speciality-12.68%</p>
<p>Adm-clerical-11.49%</p>
<p>Exec-Managerial-12.715%</p>
<p>Other Services-10.18%</p>
<p>Sales -11.33%</p>
<p>Craft-Repair -12.42%</p>
<p>Tech-support- 2.8%</p>
<p>Protective-service 2.01%</p>
<p>Farming &ndash;fishing 3.05%</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
</td>
<td width="142">
<p>The adult census income data for variable Occupation reveals that 12.68% have occupation Prof-speciality, 11.49% belong to Adm-clerical, 12.715% are Exec-Managerial,11.33% belong to Sales and 12.42% relates to Craft-Repair.</p>
<p><strong>X-axis</strong>: Occupation</p>
<p><strong>Y-axis</strong>: Frequency</p>
</td>
<td width="456">

<p align="center"><img src="https://github.com/VVRChilukoori/Income-prediction-of-a-person-using-SAS/blob/branch/img/11.jpg" alt="" width="456" height="300" /></p>

</td>
</tr>
</tbody>
</table>

<p>&nbsp;</p>
<ul>
<li><b>Data Preparation</b></li>
</ul>
<p>In preparing the data for analysis, it became immediately apparent that we needed greater consistency among our variable responses and that we also needed to address the missing values and unknown information. The data needed to be repaired, replaced, imputed and partitioned.</p>
<p>Occupation: This field identified the age of all the people. Our data revealed that 1843(or 5.66%) values were missing of total values 32561.</p>
<p>Workclass &ndash; This field identifies the workclass of all the people.Our data revealed that 1836(or 5.63%) values were missing out of total values 32561</p>
<p>Native_country-This field identifies the native country to which the person belongs to .Our data revealed that 583(1.7%) values were missing out of 32561.</p>
<ul>
<li><b>Data Modeling, Analysis and Assessments</b></li>
</ul>
<p>To identify models and assess our data, we implemented the use of Enterprise Miner. The use of each of these tools is outlined below:</p>
<ul>
<li><b>Enterprise Miner</b></li>
</ul>
<p>&nbsp;To conduct greater descriptive, inferential analysis and predictive modeling in order to identify variables that contribute to income greater than 50K, we moved our efforts to using Enterprise Miner as our data analysis tool.&nbsp; Enterprise Miner would allow us to consider decision trees, regression analysis and neural networks in identifying a final model.&nbsp; In order to complete the process, we identified the need to partition and transform the data as follows:</p>
<p>&nbsp;</p>
<ol>
<li>Replacement Node:</li>
</ol>
<p>In Replacement node we replaced values for Native_country, Occupation, Workclass variables that has &lsquo;?&rsquo; values with &lsquo;_MISSING_&rsquo; value to identify the people to which they belong to. As demonstrated in the image below of the native_country and other two has a formatted value of &lsquo;?&rsquo;, we have put a replacement value of _MISSING_ .The missing and unknown values would be resolved in the next.</p>
<p>The following figure shows the replacement values made in replacement editor of replacement node:</p>

<p align="center"><img src="https://github.com/VVRChilukoori/Income-prediction-of-a-person-using-SAS/blob/branch/img/12.jpg" alt="" width="776" height="489" /></p>

<p>The following is the output of the replacement node after the replacements being made.</p>

<p align="center"><img src="https://github.com/VVRChilukoori/Income-prediction-of-a-person-using-SAS/blob/branch/img/13.jpg" alt="" width="776" height="489" /></p>

<ol start="2">
<li>Impute Node:</li>
</ol>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; We used impute node to replace the missing values with the Impute values for Native_country,workclass and Occupation. This particular step called for imputing missing values with the mean of the non-missing values for input. We chose to impute the values to remove any prediction bias that incomplete data presents. After imputing we got the following impute values replaced with the missing values as shown in the figure.</p>
<ol start="3">

<p align="center"><img src="https://github.com/VVRChilukoori/Income-prediction-of-a-person-using-SAS/blob/branch/img/14.jpg" alt="" width="830" height="180" /></p>

<li>Data Partition node:</li>
</ol>
<p>Data partition can be done at any point i.e. before replacement and imputation or else after and here we did before replacing and imputing the missing values. In data partition we took 50% of data for training, 50% for validation and 0% testing. This partitioning of our data would allow us to use the training data to predict a target value from our input variables while using the validation data set as a means for gauging model performance.</p>
<p>The following figure give details of summary statistics of data after doing data partition:</p>

<p align="center"><img src="https://github.com/VVRChilukoori/Income-prediction-of-a-person-using-SAS/blob/branch/img/15.jpg" alt="" width="776" height="489" /></p>


<ul>
<li><b>Model Selection</b></li>
</ul>
<p>In applying our analysis, we compared the following models:</p>
<ol>
<li>Decision Tree- In order to build a predictive model to isolate cases with identical target values we implemented the use of a Decision Tree. In analyzing the results of our decision tree, we were able to identify useful input variables: Relationship was the first split and there were competing splits at education, occupation, hours_per_week and sex. There were 33 leaves in the maximal tree in the maximal tree and Average Squared Error (validation) = 0.1166</li>
</ol>
<p>Figure below shows the plots of average square error for both Train and validation data:</p>
<p>&nbsp;</p>
<p>It is evident from the decisions trees that relationship and education are the most important predictors of income.</p>
<p>At node&nbsp;&nbsp; where person enters with relationship Not-IN-FAMILY, UMMARRIED and education HS-GRAD, 7<sup>TH</sup>-8<sup>TH</sup>, SOME COLLEGE and hours_per_week &lt;41.5 or Missing the probability that a person has income&lt;50K is 97.88%. The same person has probability of income &gt;50K to be 2.112%.&nbsp;&nbsp;&nbsp;</p>
<p>At node where relationship is Not-IN-FAMILY, UMMARRIED and education is DOCTORATE,PROF-SCHOOL and age is &lt;31.5 and hours_per_week &lt;44.5 or missing the probability that a person has income &lt;50K is 97.49%. The same person has probability of income &gt;50K to be 2.51%.</p>
<p>The figure below is the full tree diagram:</p>
<p>The figure below gives the relation that is the strong indicator for target variable to be &lsquo;0&rsquo;.</p>
<p>The figure below gives the relation that is the strong indicator for target variable to be &lsquo;1&rsquo;.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<ol start="2">
<li>Regression Analysis :</li>
</ol>
<p>We implemented the use of regression analysis to identify those variables inputs that were most useful in predicting a favorable outcome of our target value &ldquo;Target&rdquo; and also to estimate the relationship among the variables.</p>
<p>The figure below gives details of the summary of step-wise selection.</p>
<p>In considering the logsworth and odd-ratio, we found that the most useful variables selected in the final model included IMP_REP_OCCUPATION, EDUCATION, REP_AGE</p>
<p>Figure below is the output from Regression node.</p>
<p>Considering occupation effect, the odds of persisting increase by 19% for each increase in &lsquo;Adm-clerical vs Transport-moving&rsquo;. More impressively odds more than double for every increase in &lsquo;Exec-managerial vs Transport-moving&rsquo; in occupation.&nbsp; Odds of persisting occupation &lsquo;0&rsquo; vs &lsquo;1&rsquo; is more than 3-times. The effect of &lsquo;sex&rsquo; role i.e. &lsquo;male vs female&rsquo; ratio is 38.3 percent.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>The results of fit statistics obtained from regression analysis is shown below.</p>
<p>The value obtained for Average square error for validation is &lsquo;0.113479&rsquo;.</p>
<p><strong>Iteration plot:</strong></p>
<p>From the above iteration plot it can be said that the values get optimized at step &lsquo;9&rsquo;.</p>
<p>&nbsp;</p>
<p>3) Neural Network -</p>
<p>We connected Neural Network node to Impute node. In implementing a neural network, our task was to identify those variables that had greatest absolute weight in predicting out target. The average square error for the validation data is 0.11101.</p>
<p>To run the &lsquo;neural network&rsquo; completely we changed the properties of neural network. Model selection Criterion was changed to Average Error.</p>
<p>In considering our input and target variables, education 10<sup>th</sup> variable had the largest absolute weight at 1.193921 and is used to calculate hidden unit 2. &nbsp;This variable was followed closely by the IMP_REP_native_coCambodia variable at 0.441876 and was also used to calculate hidden unit 3.</p>
<p>&nbsp;From the above iteration plot it can be said that the values get optimized at step &lsquo;35&rsquo;.</p>
<p><strong>4.) Neural Network2:</strong></p>
<p>We wanted to compare the results and get the lowest average square error so we tried methods. In this process we again connected the neural network to regression node and the following was observed (In fit statistics).</p>
<p>We changed the properties to the same properties that we kept for the neural network (i.e model selection Criterion was changed to Average Error).</p>
<p>From the above iteration plot it can be said that the values get optimized at step &lsquo;36&rsquo;, which is higher compared to neural network that was directly connected to impute node. So this was not a good method. So we stopped from doing further analysis on this approach.</p>
<p>5.) Auto Neural:</p>
<p>The AutoNeural is an automated tool which helps to find the optimal configurations without many inputs needed to be given to it. We tried this by connecting it to the regression node, ran it and following results were obtained (in Fit Statistics table).</p>
<p>But the values obtained were higher than normal neural network values.</p>
<p>&nbsp;</p>
<p><b>Model Comparison &amp; Model Selection:</b></p>
<p>For model comparison and selection we used the model comparison node available in the enterprise miner</p>
<p>After generating all the different models using the different nodes, we performed a model comparison using the Model comparison node. We connected all the nodes (i.e. Regression, Decision Tree, Neural Network, Neural Network (2), AutoNeural nodes) to model comparison node and ran it. The following results were obtained (in fit statistics table).</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; In applying a comparison model, it was found that Neural Network is the best model.&nbsp; It has a validation ASE = 0.11101, a validation Misclassification Rate = .159808 and the best ROC index at 0.891.</p>
<p>Below is the screenshot of our completed project showing all the nodes with diagram.</p>
<p><b>Conclusions and Recommendations:</b></p>
<p>In conclusion what did we learn from our analysis?&nbsp; Did we meet our stated business objective(s)?&nbsp; How can the results of our analysis address the business problem/opportunity?&nbsp; What further analysis that builds on our work can be done in the future.&nbsp; Our responses to each of these valid questions is noted below:</p>
<ol>
<li>While the models provided great insight in to the validity of our chosen variables on the target of income, we were unable to test our model because we did not have a viable sample of data to test. To complete the process, you must be able to test the model.</li>
<li>A number of variables, such as relationship, education, occupation, hours_per_week are determinant factors in predicting income factor less than 50K and greater than .It implies that much of the people&rsquo;s income is determined by the factor the kind of relationship a person is having. Our model determines the probability of a person&rsquo;s income based on several factors. It can help us to predict beforehand which factors contribute to income of a person greater than 50K.</li>
<li>During our analysis it was found that to determine the person having income less than 50K whose relationship is Relationship, education, hours_per_week and occupation are the biggest contributors.</li>
<li>While analyzing and looking for the patterns to predict Income less than and greater than 50K we learnt a lot in terms of usage of variables in the dataset. We also learnt for prediction which are required to be rejected and which variables are useful. We believe this is going to help us build on the knowledge of the subject and help us better insight into any dataset and prediction models.</li>
<li>Finally from the analysis we can say that a married man with higher level of education is mostly likely to earn an income more than 50K and people whose age is less than 25 years, who education is less than &ldquo;education 10<sup>th</sup>&rdquo;and were never-married are most like to earn an income of less than 50K.</li>
</ol>
