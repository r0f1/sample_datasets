
#### Sunspot Dataset `monthly-sunspot-number-zurich-17.csv` 

```Python
dataset_url = "https://raw.githubusercontent.com/r0f1/sample_datasets/master/datasets/monthly-sunspot-number-zurich-17.csv"
date_parser = lambda x: pd.datetime.strptime(x, '%Y-%m')
df = pd.read_csv(dataset_url, sep=",", parse_dates=[0], date_parser=date_parser)
df.columns = ["month", "value"]
df.head()
```

#### Employment Dataset `wisconsin-employment-time-series.csv`

```Python
dataset_url = "https://raw.githubusercontent.com/r0f1/sample_datasets/master/datasets/wisconsin-employment-time-series.csv"
date_parser = lambda x: pd.datetime.strptime(x, '%Y-%m')
df = pd.read_csv(dataset_url, sep=",", parse_dates=[0], date_parser=date_parser)
df.columns = ["month", "value"]
df.head()
```