4. Exploratory data analysis 

EDA - Distribution of sentiment classes: 

 Interpretation: The dataset is balanced after removing duplicates, with a 0.4-point gap. There is no class-imbalance problem, so accuracy is a reliable metric, and no resampling or class weights are needed. 

EDA - Movie review length distribution: 

 

Interpretation: The distribution is strongly right skewed. Most reviews are short to medium, and a few are very long. The purple overlap region covers nearly everything, meaning the two classes have almost the same length profile. 

EDA - Review length by sentiment (boxplot):  

 

Interpretation: Length does not discriminate sentiment. 

Outliers: There are many above ~500 words. Positive has the more extreme ones (up to ~2,470, versus ~1,520 for negative). Those few extreme positive reviews drag the mean slightly higher, 233 versus 230. 

EDA - Word cloud: positive reviews 

 

Interpretation: The biggest words are “br”, “the”, “of”, “in”, “is” and “a”, followed by phrases like “this movie” and “the film”.This cloud is not informative about positive sentiment. 

EDA - Word cloud: negative reviews: 

 

Interpretation: Word Cloud's default stop word list was applied here, so the function words are gone. This makes it look very different from above positive world could. Negative vocabulary is visible (“bad”, “worst”, “stupid”, “boring”, “waste”), but it is again overshadowed by generic words.  

EDA - Number of characters in texts:  

Interpretation: It repeats the length finding in character units. Both classes have the same shape: short reviews are common and very long ones are rare. 

EDA - Number of words per review (two histograms): 

 

Interpretation: It confirms plots 2 and 3, and it is largely redundant with them. 

EDA - Top 15 meaningful words: positive vs negative: 

 

Interpretation: About 11 of the 15 words are shared. The sentiment-bearing ones are: Positive: “great”, “love” and “best”. Negative: “bad”. 
