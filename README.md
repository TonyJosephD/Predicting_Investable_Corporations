# Predicting_Investable_Corporations
## The Problem:

- Corporations are constantly looking to grow and expand their businesses with the help of investors. Most of these large companies are already successful and have proven business models. In order for them to continue attracting investments, they must demonstrate healthy fundamentals. This is where corporate credit rankings from special agencies come in to play. "Credit ratings are mostly determined by financial ratios coming from balance sheets, income statements, and cash-flow statements"(Kirtan Delwadia). There are 22 ordinal ratings rating from AAA(Best to Invest) to D(Worst to Invest).

## Question and Objective:

- Can credit rankings be utilized in supervised learning to determine binary outcomes of being investable or not based on financial ratios?
- Objective: Build a supervised learning model using Corporate Credit Rankings Binary decisions as target values, to have a model capable of predicitng investable corporations that do not have those rankings established.

## The Impact

- The findings from this analysis hope to provide instant investing decisions based on current credit rankings that are clear and concise. The final result is limited to decisions based on rankings provided by a select group of agencies. It is possible that the opinions of these agencies differ from the opinions of the investing party seeking to make a decision. Additionally, at the time of this writing, the economy is fighting an inflation battle which will inevitably affect interpretations of the financial ratios used to make these investable decisions. Using this model with outdated and/or opposing agencies viewpoints could result in undesired investing decisions.

## The Data

- The data was found through Kaggle, an online community platform for data scientists. It was made available by Kirtan Delwadia, Ravi Makwana, and Dhruvil Bhatt (Full citation below). This dataset ranges from 2010-2016 which again highlights any concerns of inflation discrepancies. There a numerous features relating to financial ratios including operating margins and return on assets. Certain characteristics such as 'Sector' are categorized in multiple columns as either a label or numerical. The full credit rankings are given as well as a column for 'Binary Rating' which distinguishes an investable company as 1 when categorized as BBB- or higher and 0 when BB+ or lower.

### Kaggle data source: https://www.kaggle.com/datasets/kirtandelwadia/corporate-credit-rating-with-financial-ratios

- Authors/Creators: Makwana, Ravi and Bhatt, Dhruvil and Delwadia, Kirtan and Shah, Agam and Chaudhury, Bhaskar, How to Get Investment Grade Rating in the Age of Explainable Ai?. Available at SSRN: https://ssrn.com/abstract=4163283 or http://dx.doi.org/10.2139/ssrn.4163283

## The Analysis

- Please see the jupyter notebook file found in this repository for the complete code. There are markdown descriptions of findings, methodologies, and interpretations found throughout the notebook.

## Conclusion

- We can predict with an average accuracy of 83.5% that a company will be investable or not based on financial ratios and their given sector. Four different models were tested during this analysis, all utilizing the same data variations consisting of continuous values. Random Forest was identified as being the most superior with over 90% accuracy, however we found our final accuracy to fall lower after performing cross validation. The extent of this analysis was to determine the possibility of supervised learning based on agency corporate ratings. It has been shown that is a possibility, however parameter tuning and additional feature engineering is recommended before any deployment of such models.
