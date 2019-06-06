Building a Model to Predict Hospital Readmission Status

For this project, I used 2017 hospital data from Rush University Medical Center and Rush Oak Park Hospital. To protect patient privacy, all
datasets and code output showing data rows have been deleted. The hospital data started off with age, race, ethnicity, gender, 
Medicare Severity Diagnosis Related Group (MS-DRG) numbers, and zip code. From the Census Bureau's American Fact Finder website, 
I extracted various zip code level social economic variables such as percent below poverty, median household income, unemployment rate, 
and percent among people at least 25 years old who have a high school degree. The zip code level social economic variables were merged 
with the hospital data by zip code. In order to attain MS-DRG descriptions and categories, I web scraped Centers for Medicare & Medicaid 
Services website and merged them with the hospital dataset by MS-DRG number. 

I used unsupervised machine learning to see how the patients can be grouped by using k-means clustering. Race/ethnicity, gender, and
socio-economic status appeared to characterize the clusters. To build a predictive model, I used various supervised machine learning 
techniques, which included logistic regression, random forest, k-nearest neighbors, support vector machine, and neural network. Every model
except for the random forest had about 85-86% accuracy. 
