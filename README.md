# Santander
import pandas as pd
df = pd.read_csv('train_ver2.csv')


df.isnull().any().sum()
--out: 44

df.isnull().sum().sum()> all missing values
--out: 374489

--0.0117% is null.

i replaced null values with NA (df.fillna("NA")), then saved the file to csv file

then I deleted the null records using df.dropna()

df.duplicated() >> no duplication found

