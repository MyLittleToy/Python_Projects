# Python_Projects

Dataset:


# Step 1: import libraries
import pandas as pd
import plotly.express as px

data = pd.read_pickle('/content/ny_taxi_jan2023.pkl')

### Basic Data Exploration
# Display the first few rows of the dataset
data.head()


# Look at an overview of this dataset
data.info()
<class 'pandas.core.frame.DataFrame'>
Int64Index: 392813 entries, 0 to 413427
Data columns (total 19 columns):

 #   Column                 Non-Null Count   Dtype         
---  ------                 --------------   -----         
 0   VendorID               392813 non-null  string        
 1   tpep_pickup_datetime   392813 non-null  datetime64[ns]
 2   tpep_dropoff_datetime  392813 non-null  datetime64[ns]
 3   passenger_count        392813 non-null  float64       
 4   trip_distance          392813 non-null  float64       
 5   RatecodeID             392813 non-null  string        
 6   store_and_fwd_flag     392813 non-null  string        
 7   PULocationID           392813 non-null  string        
 8   DOLocationID           392813 non-null  string        
 9   payment_type           392813 non-null  string        
 10  fare_amount            392813 non-null  float64       
 11  extra                  392813 non-null  float64       
 12  mta_tax                392813 non-null  float64       
 13  tip_amount             392813 non-null  float64       
 14  tolls_amount           392813 non-null  float64       
 15  improvement_surcharge  392813 non-null  float64       
 16  total_amount           392813 non-null  float64       
 17  congestion_surcharge   392813 non-null  float64       
 18  airport_fee            392813 non-null  float64       
dtypes: datetime64[ns](2), float64(11), string(6)
memory usage: 59.9 MB

# Statistical summary of the dataset
data.describe()




