# HeartDisease
Loading Data

### Introduction

Heart disease affects hundreds of thousands of people a year and is the leading cause of death in the United States. There are several lifestyle choices and medical conditions that can put you at risk for heart disease including diabetes, unhealthy diet, lack of physical activity, overweight and obesity, smoking, etc. Another major risk of having heart disease is genetics CDC (2022). Analyzing this data will help in understanding the tests and other symptoms to look out for.

### Data Description
      
As seen in Table 1 there are 13 variables and 302 observations in the Heart Disease UCI data set retrieved from Kaggle.com “Heart Disease UCI” (n.d.). 

| Table 1:                |        |                                                                                                                                |
|-------------------------|--------|--------------------------------------------------------------------------------------------------------------------------------|
| Variable                | Type   | Description                                                                                                                    |
| Age                     | num    | age of patient                                                                                                                 |
| Gender                  | factor | 0 = Female                                                                                                                     |
|                         |        | 1 = Male                                                                                                                       |
| Chest Pain              | factor | chest pain:                                                                                                                    |
|                         |        |  0 = Typical Angina: chest pain related to decrease blood supply to the heart                                                  |
|                         |        |  1 = Atypical Angina: chest pain not related to the heart                                                                      |
|                         |        |  2 = non-Anginal Pain: typical esophageal spasms (not heart related)                                                           |
|                         |        |  3 = Asymptomatic: chest pain not showing signs of heart disease                                                               |
| Resting Blood Pressure  | num    | Resting blood pressure (in mm Hg on admission to the hospital) anything above 130-140 is typically cause for concern           |
| Cholesterol             | num    | Cholesterol: serum cholesterol in mg/dl (milligrams per deciliter)                                                             |
|                         |        |  serum = LDL + HDL + .2*triglycerides                                                                                          |
| Fasting Blood Sugar     | factor | Fasting blood sugar: > 120 mg/dl (milligrams per deciliter)                                                                    |
|                         |        |  1 = true                                                                                                                      |
|                         |        |  0 = false                                                                                                                     |
| Resting ECG             | factor | Resting electrocardiographic (EKG or ECG):                                                                                     |
|                         |        |  0 = nothing to note                                                                                                           |
|                         |        |  1 = ST-T Wave abnormality (can range from mild symptoms to severe problems, signals non-normal heartbeat)                     |
|                         |        |  2 = Possible or definite left ventricular hypertrophy (enlarged hearts main pumping chamber)                                  |
| Maximum Heart Rate      | num    | Maximum heart rate achieved                                                                                                    |
| Exercise Induced Angina | factor | Exercise induced angina                                                                                                        |
|                         |        |  1 = true                                                                                                                      |
|                         |        |  0 = false                                                                                                                     |
| Oldpeak                 | num    | ST depression induced by exercise relative to rest looks at stress of heart during exercise (unhealthy heart will stress more) |
| Slope                   | factor | The slope of the peak exercise ST segment                                                                                      |
|                         |        |  0 = Upsloping: better heart rate with exercise (uncommon)                                                                     |
|                         |        |  1 = Flatsloping: minimal change (typical healthy heart)                                                                       |
|                         |        |  2 = Downsloping: signs of unhealthy heart                                                                                     |
| Fluoroscopy Blood Flow  | factor | Number of major vessels colored by fluoroscopy (procedure to see blood flow)                                                   |
| Heart Disease           | char   |  0 = do not have heart disease                                                                                                 |
|                         |        |  1 = have heart disease  

There are five quantitative variables including age, resting blood pressure, cholesterol, maximum heart rate, and oldpeak. 
* The minimum age of an individual in this study is 29 years old and the maximum is 76.
* The resting blood pressure numbers represents the systolic pressure (top number) when reading blood pressure.
* The range of the observations fall between 94 and 200 with anything above 130 to 140 indicating a cause for concern.
* The cholesterol levels are derived from the formula serum = LDL + HDL + 0.2 * triglycerides. Where LDL stands for low-density lipoprotein and is typically consider the “bad cholesterol.” HDL stands fro high-density lipoprotein or the “good cholesterol.” HDL absorbs cholesterol in the blood and carries it back to the liver to be flushed from the body. Triglycerides is a type of fat in you blood that your body uses for energy. Low-levels of LDL and/or low-levels HDL with high levels of triglycerides increases the risk of health problems, like a heart attack. If the serum is greater than 200 this is typically cause for concern.
* The maximum heart rate numbers show a range between 71 and 202. People with a maximum of over 140 are more at risk of having heart disease.
* Old peak measures exercise-induced ST depression versus the heart at rest, a unhealthy heart will stress more.

There are nine categorical variables in the data including gender, chest pain, fasting blood sugar, resting electrocardiograph, exercise induced angina, slope, fluoroscopic blood flow, and the target variable heart disease. 
* There are roughly twice as many males in this study than females with 186 males and 92 females represented.
* Chest pain has four groups, the first is a typical angina, meaning the subjects have chest pain related to decrease blood supply to the heart. The second is atypical angina, which is chest pain that is not related to the heart. The non-anginal pain is typical esophageal spasms that are not related to the heart. The last group is asymptomatic chest pain with no signs of heart disease.
* Fasting blood sugar is represented by a 1 if the individual has a blood sugar of over 120 mg/dl and a 0 if the individual is below 120 mg/dl.
* Resting electrocardiographic has three groups where the first group indicates there was nothing to note from the ECG results. The second group is ST-T wave abnormality which can indicate mild to severe symptoms of a non-normal heart beat. The last group are individuals who may have a left ventricular hypertrophy, or an enlarged of the hearts main pumping chamber. This is the smallest group consisting of only three individuals, where only one was reported to have heart disease.
* Exercise induced angina is also represented by a 1 for individuals who suffer chest pain when exercising and a 0 for individuals who do not suffer chest pain when exercising.
* The slope of the peak exercise ST segment contains three groups. The first group is upsloping, which indicates a better heart rate with exercise, which is uncommon. The second group is flatsloping, this indicates minimal change in heart rate and is considered a typical healthy heart. The last group is downsloping, this is a sign of an unhealthy heart.
* Fluoroscopy blood flow measure the movement of blood in the body, the lower the number the better the blood flow or no indications of clots in the blood system.
* The last categorical variable is whether the individual has heart disease or not represented by a 1 if they have heart diseasee or 2 if they do not have heart disease.

                                                                                                      |
