The goal of this project was to process and quickly analyze a dataset. This particular dataset is data on COVID variants for countries over time. 

The original data is from this kaggle dataset: https://www.kaggle.com/yamqwe/omicron-covid19-variant-daily-cases


The cleaned data contains these columns:

location: str: the country of the data point, only the United States and Japan in the cleaned version

date: datetime: the date of the data point

variant: str: the particular variant, in the cleaned dataset only Omicron

num_sequences: int: the number of sequences on that particular country, variant, and date

perc_sequences: float: the percentage of sequences on that particular country, variant, and date

num_sequences_total: the total number of sequences for the country, variant, and date


A potential issue in the data can be seen towards the end of the graphic where there is a steep drop-off in the number of sequences. Anecdotal evidence would indicate that this is likely not accurate and more likely a side effect of the scale of the graph and data source.