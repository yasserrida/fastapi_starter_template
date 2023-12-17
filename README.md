# FastAPI starter template with MySQL and Docker

## Requirements

- Python 3.10+
- MySQL
- Docker
- Docker compose

## Installation locally
Install the required packages in your local environment
```bash
cd api

pip install -r requirements
``` 

### Setup
1. Duplicate the `.env.example` file and rename it to `.env` 


### Run It

1. Start your  app with: 
```bash
uvicorn main:app --reload
```

2. Go to [http://localhost:8000/docs](http://localhost:8000/docs).

## Setup development environment for Docker

After installation, run the following command to create a local Docker container.

```bash
docker-compose build
docker-compose up -d
```

If Docker is running successfully, the API and DB server will be launched as shown in the following:
    - API server: http://localhost:8000
    - DB server: http://localhost:3306
