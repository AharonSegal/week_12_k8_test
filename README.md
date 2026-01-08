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


main (הסרגה השירפל - היצקילפא תדבוע תיפוס)
├── feature/dockerfile
├── feature/postgres-statefulset
├── feature/postgres-service
├── feature/api-deployment
└── feature/api-service

git checkout -b feature/dockerfile
git checkout -b feature/postgres-statefulset
git checkout -b feature/postgres-service
git checkout -b feature/api-deployment
git checkout -b feature/api-deployment
git checkout -b feature/api-service

git add .
git commit -m"init"
git push -u origin feature/postgres-statefulset
