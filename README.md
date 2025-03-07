# DiabetesPredictorAPI-ngrok

This repository contains a Diabetes Prediction Machine Learning model deployed as a public API using FastAPI and ngrok, hosted in Google Colaboratory. The API allows users to input medical data and receive predictions on the likelihood of diabetes.

## Features

- **FastAPI**: For creating the API endpoints.
- **ngrok**: To expose the local server to the internet.
- **Google Colaboratory**: For running the model and the API.

## Usage

1. Clone the repository.
2. Upload the dataset CSV file (`diabetes.csv`) and the model .sav file (`diabetes_model.sav`) to the project directory.
3. Install the necessary dependencies:

   ```bash
   pip install fastapi pydantic uvicorn pyngrok fastapi-cors-middleware nest-asyncio

## Endpoints

- `/predict`: Takes input data and returns a prediction.

## Models

- Support Vector Machine (SVM) model for predicting diabetes.

## Dependencies

```python
from fastapi import FastAPI
from pydantic import BaseModel
import pickle
import json
import uvicorn
from pyngrok import ngrok
from fastapi.middleware.cors import CORSMiddleware
import nest_asyncio

