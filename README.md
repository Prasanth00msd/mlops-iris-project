#  Iris MLOps Project

##  Overview
This project demonstrates a complete MLOps pipeline:
- Model Training using Scikit-learn
- API Development using FastAPI
- Containerization using Docker
- GitHub Project Hosting

---

##  Features
- Train ML model
- Save model as pickle
- REST API for prediction
- Dockerized deployment
- Swagger documentation

---

##  Tech Stack
- Python 3.13
- FastAPI
- Scikit-learn
- Docker

---

##  How to Run

### Train Model
```
python train.py
```

### Build Docker
```
docker build -t iris-ml .
```

### Run Docker
```
docker run -p 8000:8000 iris-ml
```

Open:
http://localhost:8000/docs

---

##  Sample Prediction Request

POST /predict

```
{
  "sepal_length": 5.1,
  "sepal_width": 3.5,
  "petal_length": 1.4,
  "petal_width": 0.2
}
```
