coordinates-k8s/
├── Dockerfile
├── main.py
├── requirements.txt
├── .env.example
├── .gitignore
├── .dockerignore
├── README.md
├── k8s/
│ ├── postgres-statefulset.yaml
│ ├── postgres-service.yaml
│ ├── api-deployment.yaml
│ └── api-service.yaml
└── screenshots/
├── kubectl-get-all.png
├── kubectl-get-pods.png
├── api-response.png
└── cluster-ui.png


main
├── feature/dockerfile
├── feature/postgres-statefulset
├── feature/postgres-service
├── feature/api-deployment
└── feature/api-service

git checkout feature/dockerfile
git checkout feature/postgres-statefulset
git checkout feature/postgres-service
git checkout feature/api-deployment
git checkout feature/api-service

git add .
git commit -m"docker build"
git push 


docker build -t aharonsegal/coordinates_api:v1 .

# image name 
aharonsegal/coordinates_api:v1

