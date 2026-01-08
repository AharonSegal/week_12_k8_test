https://minikube.sigs.k8s.io/docs/handbook/
https://kubernetes.io/docs/home/
https://docs.github.com/en
https://docs.docker.com/
https://docs.docker.com/docker-hub/
https://octopus.com/devops/kubernetes-deployments/kubernetes-yaml-types/
https://medium.com/geekculture/cheatsheet-for-kubernetes-minikube-kubectl-5500ffd2f0d5


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
│ ├── coordinates-apiloyment.yaml
│ └── coordinates-api-svc.yaml
└── screenshots/
├── kubectl-get-all.png
├── kubectl-get-pods.png
├── api-response.png
└── cluster-ui.png


main
├── feature/dockerfile
├── feature/postgres-statefulset
├── feature/postgres-service
├── feature/coordinates-apiloyment
└── feature/coordinates-api-svc

git checkout main
git checkout feature/dockerfile
git checkout feature/postgres-statefulset
git checkout feature/postgres-service
git checkout feature/coordinates-apiloyment
git checkout feature/coordinates-api-svc

git add .
git commit -m"yamls"
git push 


docker build -t aharonsegal/coordinates_api:v2 .
docker push aharonsegal/coordinates_api:v2


# image name 
aharonsegal/coordinates_api:v1

git merge feature/postgres-statefulset

minikube start
kubectl get nodes
kubectl config current-context

kubectl describe 
kubectl get pods 
kubectl logs
kubectl apply -f ./k8s

kubectl describe service 
kubectl get svc        
kubectl get deploy    

minikube service api-service

kubectl delete pods --all

kubectl apply -f ./k8s

kubectl delete -f ./k8s

├───────────┼─────────────────────┼─────────────┼────────────────────────┤
│ default   │ api-service         │             │ http://127.0.0.1:41007 │
│ default   │ coordinates-api-svc │             │ http://127.0.0.1:41009 │
│ default   │ kubernetes          │             │ http://127.0.0.1:41011 │
│ default   │ postgres-svc
