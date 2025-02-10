# Number Classification API 🚀

A simple API built with **FastAPI** that takes an integer as input and returns interesting mathematical properties about the number along with a fun fact from the Numbers API.

## Table of Contents
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Deployment](#deployment)
- [License](#license)

## Features
- **Mathematical Analysis:**  
  - Checks if the number is **prime**.
  - Determines if the number is **perfect**.
  - Verifies if the number is an **Armstrong number**.
  - Determines if the number is **odd** or **even**.
  - Calculates the **digit sum**.
- **Fun Fact:**  
  - Retrieves a math-related fun fact from the [Numbers API](http://numbersapi.com/).
- **CORS Enabled:**  
  - Allows cross-origin requests.
- **JSON Responses:**  
  - Returns responses in a well-defined JSON format.
- **Provides a fun fact**


## 🚀 Features
- Publicly accessible REST API
- FastAPI framework with CORS enabled
- JSON responses
- Hosted on **Render** or deployable via **Docker**
- Integrated with NumbersAPI for fun facts

## 🛠️ Installation
 Clone the repository
```bash
git clone https://github.com/aishatoshileye/number-classification-api.git
cd number-classification-api
```

  Create a virtual environment (Optional but recommended)
```bash
python -m venv venv
source venv/bin/activate  # On macOS/Linux
venv\Scripts\activate  # On Windows
```

###  Install dependencies
```bash
pip install -r requirements.txt
```

###  Run the FastAPI server
```bash
uvicorn main:app --reload
```

###  Access API documentation
Open your browser and visit:
- **Swagger UI:** [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs)
- **ReDoc:** [http://127.0.0.1:8000/redoc](http://127.0.0.1:8000/redoc)

## 📡 API Endpoints
### 🟢 `GET /api/classify-number`
**Query Parameters:**
- `number` (int) → The number to classify

**Example Request:**
```bash
curl -X 'GET' 'http://127.0.0.1:8000/api/classify-number?number=371' -H 'accept: application/json'
```

**Example Response:**
```json
{
  "number": 371,
  "is_prime": false,
  "is_perfect": false,
  "properties": ["armstrong", "odd"],
  "digit_sum": 11,
  "fun_fact": "371 is a narcissistic number."
}
```

### 🏠 `GET /`
Returns a welcome message.

## 🌍 Deployment
### 🚀 Deploying to Render
1. Push your code to **GitHub**
2. Go to [Render](https://render.com/) and create a new **Web Service**
3. Connect your repository
4. Set **Build Command:** `pip install -r requirements.txt`
5. Set **Start Command:** `uvicorn main:app --host 0.0.0.0 --port 8000`
6. Deploy 🚀

### 🐳 Deploying with Docker
1. Build the Docker image:
```bash
docker build -t number-classification-api .
```

2. Run the container:
```bash
docker run -p 8000:8000 number-classification-api
```

## 📝 License
MIT License © 2025 Aishat Oshileye









