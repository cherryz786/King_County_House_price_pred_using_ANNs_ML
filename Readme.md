# House Sales in King County, USA - Machine Learning Project

![King County, WA](https://github.com/ishikawa-yui/King_County_House_price_pred_using_ANNs_ML/assets/71602299/0f65efeb-4c5e-41ca-b800-b61be137adcb)


Welcome to the "House Sales in King County, USA" machine learning project repository. In this project, we analyze a dataset containing house sale prices for King County, which includes Seattle, for homes sold between May 2014 and May 2015. This dataset is ideal for evaluating simple regression models.

## Dataset Details

- **Dataset Source:** [Kaggle - House Sales Prediction](https://www.kaggle.com/datasets/harlfoxem/housesalesprediction)
- **Description:** The dataset consists of the following feature columns:

   - `id`: Unique ID for each home sold.
   - `date`: Date of the home sale.
   - `price`: Price of each home sold.
   - `bedrooms`: Number of bedrooms.
   - `bathrooms`: Number of bathrooms, where 0.5 accounts for a room with a toilet but no shower.
   - `sqft_living`: Square footage of the apartment's interior living space.
   - `sqft_lot`: Square footage of the land space.
   - `floors`: Number of floors.
   - `waterfront`: A dummy variable for whether the apartment was overlooking the waterfront or not.
   - `view`: An index from 0 to 4 indicating how good the view of the property was.
   - `condition`: An index from 1 to 5 indicating the condition of the apartment.
   - `grade`: An index from 1 to 13, where 1-3 falls short of building construction and design, 7 has an average level of construction and design, and 11-13 have a high quality level of construction and design.
   - `sqft_above`: The square footage of the interior housing space that is above ground level.
   - `sqft_basement`: The square footage of the interior housing space that is below ground level.
   - `yr_built`: The year the house was initially built.
   - `yr_renovated`: The year of the house's last renovation.
   - `zipcode`: The zipcode area the house is in.
   - `lat`: Latitude.
   - `long`: Longitude.
   - `sqft_living15`: The square footage of interior housing living space for the nearest 15 neighbors.
   - `sqft_lot15`: The square footage of the land lots of the nearest 15 neighbors.

## Libraries Used

- pandas
- numpy
- matplotlib
- seaborn

## Data Preprocessing

For data preprocessing, we used the MinMaxScaler to scale the numerical features.

## Model Creation

We built a regression model using Artificial Neural Networks (ANN) with TensorFlow and Keras. The following Keras components were imported:

```python
from tensorflow.keras.models import Sequential
from tensorflow.keras.layers import Dense, Activation
```

We also used the Adam optimizer for training the model.

## Model Evaluation
To evaluate the model's performance, we utilized the following metrics:

- **mean_squared_error**: Measures the average squared difference between predicted and actual values.
- **mean_absolute_error**: Measures the average absolute difference between predicted and actual values.
- **explained_variance_score**: Measures the proportion of variance in the target variable that is explained by the model.
