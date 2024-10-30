=========================================
Dataset characteristics
=========================================	
day.csv have the following fields:
	
	- instant: record index
	- dteday : date
	- season : season (1:spring, 2:summer, 3:fall, 4:winter)
	- yr : year (0: 2018, 1:2019)
	- mnth : month ( 1 to 12)
	- holiday : weather day is a holiday or not (extracted from http://dchr.dc.gov/page/holiday-schedule)
	- weekday : day of the week
	- workingday : if day is neither weekend nor holiday is 1, otherwise is 0.
	+ weathersit : 
		- 1: Clear, Few clouds, Partly cloudy, Partly cloudy
		- 2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
		- 3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
		- 4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
	- temp : temperature in Celsius
	- atemp: feeling temperature in Celsius
	- hum: humidity
	- windspeed: wind speed
	- casual: count of casual users
	- registered: count of registered users
	- cnt: count of total rental bikes including both casual and registered

### Libraries Used
- **NumPy**: For numerical operations.
- **Pandas**: For data manipulation and analysis.
- **Seaborn** and **Matplotlib**: For data visualization.
- **scikit-learn (sklearn)**: For preprocessing, train-test splitting, feature selection, and model evaluation.
- **statsmodels**: For statistical analysis, particularly in evaluating multicollinearity.

### Dataset Description
This section provides an overview of the dataset used in the analysis, covering various attributes and their roles in the analysis.

### Data Preprocessing
- **Scaling**: `MinMaxScaler` is used to scale the features.
- **Train-Test Split**: The dataset is divided into training and testing subsets.
- **Multicollinearity Management**: Variance Inflation Factor (VIF) is calculated to manage multicollinearity among features.

### Feature Selection
- **Recursive Feature Elimination (RFE)**: Utilized to identify the most impactful features for the model.

### Model Training and Evaluation
- **Model**: Linear Regression is used to predict the target variable.
- **Metrics**: Evaluation is performed using Mean Squared Error (MSE) and R² Score to assess model performance.
"""
	
=========================================
License
=========================================
Use of this dataset in publications must be cited to the following publication:

[1] Fanaee-T, Hadi, and Gama, Joao, "Event labeling combining ensemble detectors and background knowledge", Progress in Artificial Intelligence (2013): pp. 1-15, Springer Berlin Heidelberg, doi:10.1007/s13748-013-0040-3.

@article{
	year={2013},
	issn={2192-6352},
	journal={Progress in Artificial Intelligence},
	doi={10.1007/s13748-013-0040-3},
	title={Event labeling combining ensemble detectors and background knowledge},
	url={http://dx.doi.org/10.1007/s13748-013-0040-3},
	publisher={Springer Berlin Heidelberg},
	keywords={Event labeling; Event detection; Ensemble learning; Background knowledge},
	author={Fanaee-T, Hadi and Gama, Joao},
	pages={1-15}
}

=========================================
Contact
=========================================
	
For further information about this dataset please contact Hadi Fanaee-T (hadi.fanaee@fe.up.pt)
