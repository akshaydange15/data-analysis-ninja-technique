source: code with harry

open in Visual studio code 

here we are making a report on data we get
this mehthod provide us insight about data point 


*******code******
import pandas as pd
from pandas_profiling import ProfileReport

df = pd.read_csv('data_set_name.csv')
print (df)

#generate a report
profile = ProfileReport(df)
profile.to_file(output_file = "report_name.html")