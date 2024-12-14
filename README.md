
# Credit Risk Modelling

There is an NBFC(non-banking-financial-company) company called Loki finance, which provides lones to persons who are not able to get loans from traditional banks Loki finance will get data from credit bureau then loki finance will built scoring models(ML model)-> it will tell wheather you are very strong interms of getting loan.

## Project Structure

- **artifacts/**: Contains models joblib files.
- **main**: Contains actual streamlit codes.
- **prediction_helper**: contains methods used to load models and predict the output and display it in frontend
- **requirements.txt**: Lists the required Python packages.
- **README.md**: Provides an overview and instructions for the project.

## Skills gained
- **Machine learning**
- **Data cleaning**
- **EDA**
- **Data preprocessing**


## Project Explanation

These are the steps I followed during this project:
1. Data cleaning
2. EDA (exploratory data analysis)
3. Feature Engineering
4. Hyper parameter tuning
5. Model training and evaluation
6. Rank ordering and KS statistic
7. Streamlit Deployment


The main and important points that i followed in this project is:

1. Dividing the data into train and test before starting data cleaning in order to avoid Data Leakage.
2. During featuring Engineering I checked for multicollinearity in numerical columns and removed the columns which are highly correlated.
3. I used IV(information value) and WOE(weight of Evidence) to check how much a categorical feature is contributing to the target feature.
4. Used Optuna for hyperparameter tuning which is efficient than grid search and random search.

5. At last after model training , i calculated KS statistic and verified whether my model's KS statistic falls 
 under top 3 deciles which means my model is better at differentiating default and non-default 
 classes.


## Authors

- [@siddu28](https://github.com/siddu28/ML-project-credit-risk-model)


## Demo

https://ml-project-credit-risk-modeling.streamlit.app/


## Screenshots

![App Screenshot](https://github.com/siddu28/ML-project-credit-risk-model/blob/main/Screenshot%202024-11-25%20230508.png)

## Demo video
https://github.com/user-attachments/assets/211760da-1142-4260-93a0-6526fbb9ea39


## Setup Instructions

1. **Clone the repository**:
   ```bash
   https://github.com/siddu28/ML-project-credit-risk-model.git

1. **Install dependencies:**:   
   ```commandline
    pip install -r requirements.txt
   ```

1. **Run the Streamlit app:**:   
   ```commandline
    streamlit run main.py
   ```
    
