## Assignment 1: Data Collection and Curation

The goal of this project was to process and quickly analyze a dataset. This particular dataset is data on COVID variants for countries over time. After cleaning the dataset, analysis is done comparing the amount of virus sequences in the US to Japan. This is to see if there is a difference in how dramatically the countries see a spike in the Omicron variant, which can potentially inform future pandemic responses based on differences in policy between the countries.

The original data is from this kaggle dataset: https://www.kaggle.com/yamqwe/omicron-covid19-variant-daily-cases


The cleaned data contains these columns:
* location: str - the country of the data point, only the United States and Japan in the cleaned version
* date: datetime - the date of the data point
* variant: str - the particular variant, in the cleaned dataset only Omicron
* num_sequences: int - the number of sequences on that particular country, variant, and date
* perc_sequences: float - the percentage of sequences on that particular country, variant, and date
* num_sequences_total: int - the total number of sequences for the country, variant, and date


A potential issue in the data can be seen towards the end of the graphic where there is a steep drop-off in the number of sequences. Anecdotal evidence would indicate that this is likely not accurate and more likely a side effect of the scale of the graph and data source. Furthermore, there is potentially a bias when viewing the difference between the US and Japan. The US has much more cases - partly of which is a product of its much higher population. When performing further analysis on the data, more attention should be paid towards the trends that the data follows, rather than the pure volume of sequences.