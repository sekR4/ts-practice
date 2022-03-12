# ts-practice
Some experimentation with time series data

## Data
```bash
# https://archive.ics.uci.edu/ml/datasets/Online+Retail+II
curl -o src/data/online_retail_II.xlsx -O https://archive.ics.uci.edu/ml/machine-learning-databases/00502/online_retail_II.xlsx

# https://archive.ics.uci.edu/ml/datasets/Individual+household+electric+power+consumption
project=household_power_consumption
url=https://archive.ics.uci.edu/ml/machine-learning-databases/00235/$project.zip
curl -o $project.zip -O $url && unzip $project.zip && rm $project.zip && mv $project.txt src/data
```

## Environment
```bash
pyenv virtualenv 3.8.10 tseries
pyenv activate tseries
pip install -U pip && pip install -r requirements.txt
```