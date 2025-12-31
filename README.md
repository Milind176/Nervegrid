# AWS Costing Summary

A Python application for scraping and analyzing AWS cost data using boto3 and storing insights in MongoDB.

## Features

- AWS Cost Explorer integration using boto3
- Environment-based configuration for AWS credentials
- MongoDB integration for data storage
- FastAPI backend for APIs
- AI-powered cost analysis and insights

## Prerequisites

- Python 3.8 or higher
- AWS Account with appropriate permissions
- MongoDB instance (local or cloud)

## Setup Instructions

### 1. Clone Repository
Clone the repo

### 2. Create Virtual Environment
```bash
python3 -m venv venv
```

### 3. Activate Virtual Environment
```bash
source venv/bin/activate
```

### 4. Install Dependencies
```bash
pip install -r requirements.txt
```

### 5. Environment Configuration
Copy the example environment file and configure your credentials:
```bash
cp .env.example .env
```

Edit the `.env` file with your actual credentials:
```bash
# AWS Configuration
AWS_ACCESS_KEY_ID=your_actual_aws_access_key_id
AWS_SECRET_ACCESS_KEY=your_actual_aws_secret_access_key
AWS_REGION=us-east-1

# MongoDB Configuration
MONGO_URL=mongodb://localhost:27017
MONGODB_DB=aws_costing
MONGODB_COLLECTION=cost_data
```

### 7. Run the Application
```bash
uvicorn main:app --reload --host 0.0.0.0 --port 8000
```

## Development

### Activate Development Environment
```bash
source venv/bin/activate
```

### Install Development Dependencies
```bash
pip install -r requirements.txt
```

### Deactivate Environment
```bash
deactivate
```

### Swagger URL
```
http://localhost:8000/docs#/
```

### steps for testing AI response
Currently AWS cost API data will get load to Model
1. Call AWS cost api it will give response as well as load data to Model
2. Then you can call Query API with your API
3.



### Connect to instance
###### Connect
`ssh -i AI-SaaS-backend.pem ec2-user@13.203.214.31`

###### Docker logs
`docker logs -f ai-saas`

# Nervegrid
# Nervegrid
