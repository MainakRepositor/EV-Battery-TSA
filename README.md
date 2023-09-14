# Battery State of Charge Prediction

Predict battery state of charge (SOC) using machine learning. Use the Streamlit web app easily browse available models and predict SOC on cell dischrage data.

Models are built using Tensorflow and trained on ***[LG 18650HG2](https://data.mendeley.com/datasets/cp3473x7xv/3)*** and ***[Panasonic 18650PF](https://data.mendeley.com/datasets/wykht8y7tg/1)*** Li-ion battery datasets.

## Repository Contents
- `datasets/`: Download datasets and load into this folder as 'LG_18650HG2' and 'Panasonic_18650PF'. 
- `training/`: Jupyter notebooks to analyze and train DNN, CNN, and LSTM models.
- `training/model_evals`: Compare model performance.
- `pre-trained/`: Pre-trained DNN, CNN, and LSTM models.
- `app/`: Streamlit app that allows users to play with their own data using the pre-trained models.

## Convert MAT to CSV
Use the `/training/panasonic/convert_mat_to_csv.ipynb` notebook to convert MAT files to CSV. Useful for the Panasonic dataset where only MAT files are available.

## Usage
To get started
- Clone this repository to your local machine.
- Download datasets, locate them under the 'datasets' folder.
- Convert Panasonic .mat files to .csv.
- Run training notebooks, or use pre-trained models.
- Navigate to `app` folder and run Streamlit app `streamlit run soc_app.py`.
- To deploy to Streamlit Cloud visit [soc-cloud-app](https://github.com/sautee/soc-cloud-app).



## Other Research Areas
**Battery Surface Temperature Estimation** - using the [Panasonic 18650PF](https://data.mendeley.com/datasets/wykht8y7tg/1) dataset used here.

**Predicting Battery Remaining Useful Life** - using data from [TRI](https://data.matr.io/1/projects/5c48dd2bc625d700019f3204), [NASA Prognostics](https://www.nasa.gov/content/prognostics-center-of-excellence-data-set-repository), [UNIBO PowerTools Dataset](https://data.mendeley.com/datasets/n6xg5fzsbv/1).
- [petermattia/predicting-battery-lifetime](https://github.com/petermattia/predicting-battery-lifetime)
- [michaelbosello/battery-rul-estimation](https://github.com/MichaelBosello/battery-rul-estimation)

