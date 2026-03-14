<h3 align="center">Churn AI : Customer Churn Prediction</h3>

<div align="center">

[![Live Demo](https://img.shields.io/badge/Live-Demo-00C7B7?style=flat&logo=netlify&logoColor=white)](YOUR_NETLIFY_LINK)
[![API Docs](https://img.shields.io/badge/API-Docs-009688?style=flat&logo=fastapi&logoColor=white)](YOUR_FASTAPI_DOCS_LINK)
[![Docker Hub](https://img.shields.io/badge/Docker%20Hub-Image-2496ED?style=flat&logo=docker&logoColor=white)](YOUR_DOCKER_IMAGE_LINK)
[![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)](https://www.python.org/)
[![Scikit-Learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat&logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)
[![MLflow](https://img.shields.io/badge/MLflow-0194E2?style=flat&logo=mlflow&logoColor=white)](https://mlflow.org/)
[![uv](https://img.shields.io/badge/uv-Astral-D7FF64?style=flat)](https://docs.astral.sh/uv/)
[![React](https://img.shields.io/badge/React-333A45?style=flat&logo=react&logoColor=61DAFB)](https://react.dev/)
[![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)](https://git-scm.com/)

</div>

<a href="#"><img title="Churn AI : Customer Churn Prediction" src="https://github.com/jacobcode01/Pickify/blob/addb7b9824a1db0cbf334f7373553382b6f45dc8/borderful.png"></a>

<hr>

## Folder Structure

```
Churn AI/
│
├── api/                          # FastAPI backend for serving model predictions
│   ├── main.py                   # API endpoints (root, health, info, predict)
│   ├── schema.py                 # Pydantic schemas for request/response validation
│   ├── config.py                 # API configuration utilities
│   ├── utils.py                  # Helper functions used by the API
│   └── Dockerfile                # Docker configuration for building API image
│
├── artifacts/                    # Saved model artifacts and evaluation metrics
│   ├── models/
│   │   └── pipe.joblib           # Trained Scikit-learn pipeline used for prediction
│   │
│   └── metrics/
│       └── metrics.json          # Model evaluation results and training metadata
│
├── configs/                      # YAML configuration files used across the project
│   ├── artifacts-config.yaml     # Artifact storage configuration
│   ├── data-config.yaml          # Dataset paths and data settings
│   ├── model-config.yaml         # Model configuration and threshold settings
│   └── training-config.yaml      # Training parameters and evaluation settings
│
├── data/                         # Project datasets
│   ├── raw/
│   │   └── customer-churn-raw.csv        # Original dataset
│   │
│   └── processed/
│       └── customer-churn-clean.parquet  # Cleaned dataset used for training
│
├── frontend/                     # React frontend for user interaction
│   │
│   ├── public/                   # Static assets used in the frontend
│   │   ├── favicon.svg
│   │   ├── hero-image.png
│   │   └── logo.png
│   │
│   ├── src/                      # React application source code
│   │   ├── App.jsx
│   │   ├── App.css
│   │   ├── main.jsx
│   │   ├── index.css
│   │   │
│   │   └── assets/
│   │       └── react.svg
│   │
│   ├── Dockerfile                # Docker configuration for frontend container
│   ├── nginx.conf                # Nginx configuration for serving frontend
│   ├── package.json              # Node.js dependencies
│   ├── package-lock.json
│   ├── index.html
│   ├── vite.config.js
│   ├── eslint.config.js
│   └── .env.example              # Example environment variables
│
├── notebooks/                    # Jupyter notebooks for experimentation
│   ├── eda.ipynb                 # Exploratory data analysis
│   ├── model.ipynb               # Model experimentation and MLflow tracking
│   └── ...                       # Additional research notebooks
│
├── scripts/                      # Executable pipeline scripts
│   ├── run_preprocessing.py      # Data preprocessing pipeline
│   └── run_training.py           # Model training pipeline
│
├── src/                          # Core machine learning pipeline implementation
│   │
│   └── customer_churn/
│       │
│       ├── core/                 # Core utilities used across the project
│       │   ├── __init__.py
│       │   ├── config.py         # Configuration loader
│       │   └── logger.py         # Logging setup
│       │
│       ├── data/                 # Data loading and preprocessing logic
│       │   ├── __init__.py
│       │   ├── loaders.py
│       │   ├── preprocessing.py
│       │   └── export.py
│       │
│       ├── features/             # Feature engineering utilities
│       │   ├── __init__.py
│       │   └── split.py
│       │
│       └── models/               # Model training and evaluation modules
│           ├── __init__.py
│           ├── pipeline.py
│           ├── preprocessor.py
│           ├── model_factory.py
│           ├── evaluation.py
│           ├── persistence.py
│           └── target_encoding.py
│
├── docker-compose.yaml           # Docker orchestration for API and frontend
├── Makefile                      # Project commands (training, MLflow, API, etc.)
├── pyproject.toml                # Python project configuration
├── uv.lock                       # Dependency lock file
├── mlflow.db                     # MLflow experiment tracking database
├── netlify.toml                  # Netlify deployment configuration
├── run.sh                        # Shell script to run project tasks
│
├── .dockerignore                 # Files ignored while building Docker images
├── .gitignore                    # Files ignored by Git
├── .python-version               # Python version specification
├── .env.example                  # Example environment variables
│
└── README.md                     # Project documentation
```

<hr>

## License

This project is licensed under the [MIT License](LICENSE). You are free to use and modify the code as needed.

<div align='left'>
  
**[`^        Scroll to Top       ^`](#churn-ai--customer-churn-prediction)**

</div>
