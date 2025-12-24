# IT-Ticket-Classifier
AI-powered it ticket classifier to automatically assign IT support tickets to specific teams and assist with the triage.


## Why This Project Exists
it front desk teams sometimes are not able to transfer the tickets correctly to the rensponsible team in real time or they lack the historical context based on past tickets to make the right decision. Also this is a perfect example of a manual task that can be automated with the help of AI.

## What it Does (Current State)
At this stage, the project focuses on building a basic but complete NLP classification pipleine.

Current capabilities:
- Accepts raw IT ticket text or JSON as input
- Cleans and preprocesses text(lowercasing, tokenization, noise removal)
- Encodes text into numberical features
- Predicts a ticket category or team name from predefined label set


## Planned Features
- 


## Tech Stack
- Language: Python
- ML/NLP: scikit-learn / PyTorch
- Data Processing: pandas, NumPy, FastAi
- API: FastAPI
- Dev Tools: Git, Github, Docker, AWS 

## Project Structure
```
    app
├── __pycache__
│   └── main.cpython-313.pyc
├── api
│   ├── __pycache__
│   │   └── health.cpython-313.pyc
│   └── health.py
├── core
├── main.py
├── models
└── services
```


## API Endpoints

### Health Check
GET /api/v1/health

## Getting Started

### Running Locally
`uvicorn app.main:app --reload`


### Prerequisites
    - Python 3.9+
    - pip

### Installation
`git clone https://github.com/surindersingh1699/it-ticket-classifier.git
cd it-ticket-classifier
`

## Usage
Example usage (early-stage CLI test):
`python src/classify_ticket.py "VPN connection drops frequently after login"`

Example output:
`Predicted category: Network
Confidence: 0.82`
This interface will evolve as the project matures

## Learning
This project is intentionally built as a learning-focused project

- Understand NLP pipelines end to end
- Practice ML model training and evaluation
- Design a real-world IT automation use case
- Transition toward AI-focused engineering roles

## License
MIT License
