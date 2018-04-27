# The Secret to Good Red Wine

<p>What makes a good wine? Could acidity change the quality of a wine? 
How about alcohol? pH level? Could any component of a wine determine 
its greatness?</p>

<p>In this project, I've analyzed which chemical properties produced a good red 
wine. The dataset contains red wines with the chemical properties of the wine.
At least 3 wine experts rated the quality of each wine, providing a rating 
between 0 (very bad) and 10 (very excellent). My goal was to look at the levels 
of each attribute of these wines with their ratings to find some patterns and 
find the key elements to good red wines.</p>

<p>Download dataset</p>

<p>The data set contains 1,599 red wines with 11 variables on the chemical 
properties of the wine. At least 3 wine experts rated the quality of each wine, 
providing a rating between 0 (very bad) and 10 (very excellent).</p>

<p>Input variables (based on physicochemical tests):<br>
   1 - fixed acidity (tartaric acid - g / dm^3)<br>
   2 - volatile acidity (acetic acid - g / dm^3)<br>
   3 - citric acid (g / dm^3)<br>
   4 - residual sugar (g / dm^3)<br>
   5 - chlorides (sodium chloride - g / dm^3<br>
   6 - free sulfur dioxide (mg / dm^3)<br>
   7 - total sulfur dioxide (mg / dm^3)<br>
   8 - density (g / cm^3)<br>
   9 - pH<br>
   10 - sulphates (potassium sulphate - g / dm3)<br>
   11 - alcohol (% by volume)<br>
   Output variable (based on sensory data): <br>
   12 - quality (score between 0 and 10)</p>
   
<p>When I first chose this detaset, I had an assumption that these attributes 
would somehow have direct influence on wine quality. However, all the 
correlation were from weak to moderate, and the strongest correlation was 
with alcohol. The distribution showed that most wines were rated 5 and 6, and in 
order to see the better difference in what makes wines good and bad, I've 
removed those two qualities from the dataset and compared the highest and lowest 
ones. Only then I saw which attributes were correlated with bigger difference 
between the "excellent" and "poor". Attributes that had strong correlations with 
excellent wine was:<br><br>
- Higher alcohol<br>
- Lower volatile acidity<br>
- Higher citric acid <br>
- Higher sulphates</p>

<p>I then decided to investigate relationships of attributes, and I saw much 
stronger correlation in them. In the corelation plot, the ones with the 
strongest correlations were:<br><br>
- pH and fixed acidity<br>
- Density and fixed acidity <br>
- Total sulfur dioxide and free fulfur dioxide<br>
- Citric acid and fixed acidity</p>

<p>When compared with the quality, ones with density had the strongest 
correlation. This is understandable since it's influenced by the percent alcohol 
and sugar content. The trend in their relationships are:<br><br>
- The lower the alcohol level, the higher the density is, while the wines with 
higher alcohol level tend to be better in quality.<br>
- The higher the density, the higher the fixed acidity, while the wines with 
higher fixed acidity tend to be better in quality.</p>

<p>The issue became more and more evident as I moved along in the process. The 
quality judged by people are not absolute, however experts they are in the field. 
And flavors of wine are so complex and interwined with each attribute that it is 
very difficult to determin what exactly makes good or bad wine. But perhaps with 
more observations, it would become more possible to make predictions.</p> 

