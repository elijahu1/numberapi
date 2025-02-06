
---

# Number Classification API 🧮

A serverless API that analyzes numbers and returns their mathematical properties, powered by AWS Lambda and NumbersAPI.

## Features ✨
- **Number Classification**: Checks if a number is prime, perfect, or Armstrong.  
- **Fun Facts**: Fetches interesting trivia from NumbersAPI.  
- **Lightning Fast**: Response time < 500ms.  
- **CORS Ready**: Works seamlessly with frontend apps.  

## Usage 🚀
### Endpoint
```bash
GET /api/classify-number?number=<integer>
```

### Example Request
```bash
curl "https://7mu12vr223.execute-api.eu-west-1.amazonaws.com/dev/api/classify-number?number=371"
```

### Example Response
```json
{
    "number": 371,
    "is_prime": false,
    "is_perfect": false,
    "properties": ["armstrong", "odd"],
    "digit_sum": 11,
    "fun_fact": "371 is an Armstrong number because 3^3 + 7^3 + 1^3 = 371"
}
```

## Tech Stack 💻
- **AWS Lambda**: Serverless compute.  
- **API Gateway**: HTTP endpoint management.  
- **Python 3.13**: Backend logic.  
- **NumbersAPI**: Fun number facts.  

## Setup 🛠️
1. Clone the repo:
   ```bash
   git clone https://github.com/elijahu1/numberapi.git
   ```
2. Deploy to AWS:
   - Install AWS CLI and configure credentials.  
   - Run `deploy.sh` to deploy the Lambda function and API Gateway.  

## Contributing 🤝
Feel free to open issues or submit PRs! Check out the [contribution guide](CONTRIBUTING.md) for details.

## License 📜
MIT License. See [LICENSE](LICENSE) for details.

---
