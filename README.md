# Weather Microservice

This is a simple Python-based microservice built with **FastAPI** to fetch weather data for a given city. The service integrates with the OpenWeatherMap API to provide current weather details, such as temperature, humidity, and a brief description.

## Features
- Fetch weather data for any city.
- Lightweight and fast thanks to FastAPI.

## Requirements
- Python 3.10 or later
- OpenWeatherMap API Key

## Setup and Installation

### 1. Clone the Repository
```bash
git clone https://github.com/alvin159/Sustainable-software-engineering.git -b exercise-2
cd Sustainable-software-engineering
```

### 2. Create and Activate a Virtual Environment
We recommend using a **Jupyter Notebook** for this project. To set up your environment, do the following:

#### Install required packages
```bash
pip install fastapi uvicorn requests jupyter
```

#### Open Jupyter Notebook
Start the Jupyter Notebook in your project directory:
```bash
jupyter notebook
```

Inside the Jupyter Notebook, you can write and execute the microservice code directly.

### 3. Set Your OpenWeatherMap API Key
Replace the placeholder `your_openweathermap_api_key` in the code with your actual API key. You can obtain one by signing up at [OpenWeatherMap](https://openweathermap.org/).

### 4. Start the FastAPI Server
Run the code inside Jupyter Notebook terminal to start the server:
```bash
uvicorn main:app --reload
```

The server will run at `http://127.0.0.1:8000`.

### 5. Test the Endpoint
Access the `/weather/{city}` endpoint in your browser or use a tool like `curl` or Postman. Replace `{city}` with the name of the city you want to query. For example:
```bash
http://127.0.0.1:8000/weather/London
```

## Example Response
For a request to `/weather/London`, the API might return:
```json
{
    "city": "London",
    "temperature": 15.3,
    "humidity": 87,
    "description": "Light rain"
}
```

