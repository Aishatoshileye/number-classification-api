# Number Classification API 🚀

A simple API built with **FastAPI** that takes an integer as input and returns interesting mathematical properties about the number along with a fun fact from the Numbers API.

## Table of Contents
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Deployment](#deployment)
- [License](#license)

 Features
- Mathematical Analysis: 
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

Installation

Prerequisites
- Python 3.8+
- Git

Steps

1. **Clone the repository:**
   ```bash
   git clone https://github.com/aishatoshileye/number-classification-api.git
   cd number-classification-api


API Endpoints
GET /api/classify-number?number=371
Response:

json
{
    "number": 371,
    "is_prime": false,
    "is_perfect": false,
    "properties": ["armstrong", "odd"],
    "digit_sum": 11,
    "fun_fact": "371 is an Armstrong number because 3^3 + 7^3 + 1^3 = 371"

}
Deployment
Check out the live API: (https://number-classification-api-qm2r.onrender.com)



