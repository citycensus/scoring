# Scoring

## Overall Rank
40% Standardized Dataset Score Rank  
20 % Standardized Category Rank  
15 % Standardized Category Variance Rank  
10% Standardized Dataset Rank  
5 % Standardized Formats Rank  
5% Standardized last update rank  
5 % Standardized category rank  

The standardized ranks are multiplied by their respective weight which then results in the overall score. These scores are then ranked again.
The lower the score the better the city is performing.

__Example:__  

|Score|City 1|City 2|
|----|:---:|:---:|
|Dataset Score Rank|1|2|
|Category Rank|1|2|
|Category Variance Rank|1|2|
|Datastes Rank|1|2|
|Formats Rank|1|2|
|Last Update Rank|1|2|
|Category rank|1|2|
|Weighted Score|0.4\*1 + 0.2\*1 +0.15\*1 +0.1\*1 +0.05\*1 +0.05\*1 +0.05\*1 = **1**|0.4\*2 + 0.2\*2 +0.15\*2 +0.1\*2 +0.05\*2 +0.05\*2 +0.05\*2 = **2**|
|Resulting Rank|1|2|



### Dataset Score

The dataset score consists of the following:  
Each dataset is assigned a score. The perfect score for a dataset is 3.   
The sum of all dataset scores is divided by the number of datasets to get the resulting score  

#### Detail Dataset Score
Each dataset is scored by three criteria:
- License
- Format
- Update time

##### License
If the dataset has an open license it gets 1 point. Otherwise 0

##### Format
If the dataset has resources with an open and machine readable format it gets 1 point.
For just open or machine readable it gets 0.5 points.
Otherwise 0 points.

##### Update time
If the dataset was updated in the last 7 days it gets 1 point.
If it was updated in the last 30 days it gets 0.5 points.
Otherwise 0 points.

**Example**  

|Score|License|Format|Updated|Result|
|----|:---:|:---:|----|
|Dataset 1|Open = **1** |Machine Readable = 0.5|3 days ago = 1|1+0.5+1 = **2.5**|
|Dataset 2|Closed License = **0**|Machine Readable + Open Format = **1** | Updated 32 days ago = **0.5**|0+1+0.5 = **1.5**|


10 Datasets with a perfect score of 3 would result in a score if 3 (10\*3/10)

Afterwards all dataset scores are rank among all cities. So the city with the best score is in 1st place and so forth.

### Category Score

The category score is a score of maximum 1 one. 1 point is awarded if the city has a dataset in each category. 0,5 point if a dataset in at least half of the categories exists.

### Category Variance Score

This score computes the variance for the amount of datasets per category. If a city has a lot of datasets in just one category a low variance is the result and vice versa. A low variance is what we score highest.

### Dataset Score

The more datasets the city has, the higher the score and the rank.

### Formats Rank

The more formats the more points and rank.

### Standardization
Each rank is standardized.  
The place is divided by the maximum rank (ties are allowed) and multiplied by 100.

_Example_

Rank: 1  
Max Rank: 100  
Standardized Rank: 1  

Rank: 10  
Max Rank: 80  
Standardized Rank: 12,5  
