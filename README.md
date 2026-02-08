# user-service

User authentication and management

## 🚀 Quick Start

```bash
# Install dependencies
pip install -r requirements.txt

# Run locally  
python src/main.py

# Server starts on http://localhost:8001
```

## 🐳 Docker

```bash
# Build image
docker build -t user-service:v1 .

# Run container
docker run -p 8001:8001 user-service:v1
```

## ☸️ Kubernetes Deployment

```bash
# Deploy with Helm
helm install user-service ./helm \
  --namespace ecommerce \
  --create-namespace

# Port forward to test
kubectl port-forward svc/user-service 8001:8001 -n ecommerce
```

## 📁 Project Structure

```
user-service/
├── src/
│   ├── main.py          # Application entry point
│   ├── models/          # Data models
│   ├── routes/          # API routes
│   └── utils/           # Utilities
├── tests/               # Test files
├── helm/                # Helm chart
├── Dockerfile           # Container definition
└── requirements.txt     # Python dependencies
```

## 🔧 Configuration

Environment variables:
- `DATABASE_URL` - Database connection string (if applicable)
- `PORT` - Service port (default: 8001)
- Other service-specific configs

## 🛠️ Tech Stack

- Python 3.11
- FastAPI
- SQLAlchemy (if database)
- PostgreSQL (if database)
- Pydantic

## 📊 API Documentation

Once running, visit: http://localhost:8001/docs
# user-service
