# HousePrice_Prediction

## 1. Set up virtual enviroment
`` python -m venv venv `` <br/>
`` venv\Scripts\Activate.ps1 `` <br/>
`` python -m pip install --upgrade pip `` <br/>
`` pip install ipykernel `` <br/>
`` python -m ipykernel install --user --name=venv `` <br/>

## 2. Install Dependencies
`` pip install requirements.txt ``

## 3. Make API Calls

### 3.1 Runnung on the Local Host
`` cd app `` <br/>
`` uvicorn api:app --reload `` <br/>

API calls can be made using following structure:
POST http://127.0.0.1:8000
body: <br/>

``{ 
    "TransactionDate":"2020.12",
    "HouseAge":9.0,
    "DistanceToStation":467.6447748,
    "NumberOfPubs":10.0,
    "PostCode":"5222.0"
}``

The API will return a prediction:  <br/>
``{"prediction": 680871}``
