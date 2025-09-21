# Hotel Booking Cancellation Prediction with Machine Learning

This repository contains an end-to-end data science project, from data preprocessing and model training to the deployment of an interactive web application for predicting hotel booking cancellations.

## Project Background

Booking cancellations are a significant challenge in the hospitality industry, leading to revenue loss and difficulties in resource management. This project aims to build an accurate machine learning classification model to identify bookings with a high probability of being canceled. With this model, hotels can take proactive measures to mitigate cancellation risks.

## Project Workflow

The project was executed through several key stages:

1.  **Data Exploration and Preprocessing**: The raw dataset was cleaned, missing values were handled, and categorical features were converted into a numerical format through encoding.
2.  **Model Training and Comparison**: Two powerful classification algorithms, **Random Forest** and **XGBoost**, were trained on the preprocessed data. The performance of both models was evaluated and compared to select the best one.
3.  **Model Serialization**: The best-performing model was serialized into a file using `pickle`/`joblib` to be reused for future inference processes.
4.  **Object-Oriented (OOP) Implementation**: To improve code readability, scalability, and reusability, the entire model training workflow was refactored into an Object-Oriented Programming (OOP) structure.
5.  **Inference Script Creation**: A dedicated script (`inference.py`) was developed to load the saved model and use it to make predictions on new data.
6.  **Web Application Deployment**: The model was deployed as an interactive web application using **Streamlit**, allowing users to input new booking details and receive real-time cancellation predictions.

## How to Run the Streamlit Application

To run the prediction application locally, follow these steps:

1.  **Clone the Repository**
    ```bash
    git clone [https://github.com/your-username/your-repository-name.git](https://github.com/your-username/your-repository-name.git)
    cd your-repository-name
    ```

2.  **Install Dependencies**
    Ensure you have Python installed. Then, install all the required libraries.
    ```bash
    pip install -r requirements.txt
    ```
    *(Note: You will need to create a `requirements.txt` file containing libraries such as pandas, scikit-learn, xgboost, streamlit, etc.)*

3.  **Run the Streamlit App**
    Use the following command in your terminal:
    ```bash
    streamlit run streamlit.py
    ```

4.  The application will automatically open in your web browser. Enter the booking details you wish to test to see the prediction result.

## Technologies Used

* **Analysis & Modeling**: Pandas, Scikit-learn, XGBoost
* **Serialization**: Pickle, Joblib
* **Deployment**: Streamlit
* **Environment**: Python, Jupyter Notebook
