# Battery State of Charge Prediction

![image](https://github.com/MainakRepositor/EV-Battery-TSA/assets/64016811/2e7333bf-5fe2-4250-adfd-5cdc35f991ea)

Predict battery state of charge (SOC) using machine learning. Use the Streamlit web app easily browse available models and predict SOC on cell dischrage data.

Models are built using Tensorflow and trained on ***[LG 18650HG2](https://data.mendeley.com/datasets/cp3473x7xv/3)*** and ***[Panasonic 18650PF](https://data.mendeley.com/datasets/wykht8y7tg/1)*** Li-ion battery datasets.

## Repository Contents
- `datasets/`: Download datasets and load into this folder as 'LG_18650HG2' and 'Panasonic_18650PF'. 
- `training/`: Jupyter notebooks to analyze and train DNN, CNN, and LSTM models.
- `training/model_evals`: Compare model performance.
- `pre-trained/`: Pre-trained DNN, CNN, and LSTM models.
- `app/`: Streamlit app that allows users to play with their own data using the pre-trained models.
