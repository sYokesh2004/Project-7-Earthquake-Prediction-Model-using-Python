# Project-7-Earthquake-Prediction-Model-using-Python.
This project aims to predict earthquake magnitudes based on latitude, longitude, and depth using a Random Forest regression model. The prediction model is exposed as a Flask API for real-time predictions.

## Dataset Source

The dataset used in this project was obtained from the https://www.kaggle.com/datasets/usgs/earthquake-database, a comprehensive database maintained by the United States Geological Survey (USGS). The dataset contains historical earthquake records with essential features such as latitude, longitude, depth, and magnitude.

# how to run the code and any dependency: 
# How to Run:
  insatll jupyter notebook in your commend prompt
    # pip install jupyter lab
    # pip install jupyter notebbok (or)
        1.Download Anaconda community software for desktop
        2. Install the anaconda community
        3. open jupyter notebook
        4.type the code & execute the given code

## Dataset Description

The dataset provides information about earthquake events worldwide, including:

- **Latitude:** The geographical north-south coordinate of the earthquake location.
- **Longitude:** The geographical east-west coordinate of the earthquake location.
- **Depth:** The depth at which the earthquake occurred beneath the Earth's surface.
- **Magnitude:** The magnitude of the earthquake, indicating its energy release.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [API Endpoint](#api-endpoint)
- [Example Request](#example-request)
- [Dependencies](#dependencies)
- [License](#license)

## Prerequisites

Before running the code, ensure you have the following installed on your system:

- Python 3.x
- `pip` (Python package manager)

## Installation

1. Clone the repository to your local machine:

   ```bash
   git clone https://github.com/sYokesh2004/Project-7-Earthquake-Prediction-Model-using-Python.git
   ```

2. Navigate to the project directory:

   ```bash
   cd earthquake-prediction
   ```

3. Install the required Python packages using `pip`:

   ```bash
   pip install -r requirements.txt
   ```

## Usage

Run the Flask API server with the following command:

```bash
python earthquake_prediction.py
```

The API will be accessible at `http://localhost:5000`.

## API Endpoint

- **Endpoint:** `/predict`
- **Method:** POST
- **Request Format:** JSON
- **Request Parameters:**
  - `Latitude` (float): Latitude of the location.
  - `Longitude` (float): Longitude of the location.
  - `Depth` (float): Depth of the earthquake event.
- **Response Format:** JSON
- **Response Parameter:**
  - `Magnitude` (float): Predicted earthquake magnitude.

## Example Request

```json
{
  "Latitude": 34.0522,
  "Longitude": -118.2437,
  "Depth": 10.0
}
```

## Dependencies

- `pandas`
- `scikit-learn`
- `joblib`
- `flask`

Install these dependencies using the provided `requirements.txt` file:

```bash
pip install -r requirements.txt
```

## License

This project is licensed under the [MIT License](LICENSE).



