# microservices-nodejs-react
## Setup

Create the docker images:
`docker build -t <repo>/<entity> .`

Configure the kubernetes deployments:
`cd infra\k8s\`
`kubectl apply -f .`

Install NGINX ingress controller:
`kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/controller-v1.1.1/deploy/static/provider/cloud/deploy.yaml`

## Usefull
Restart kubernetes deployments:
`kubectl rollout restart deployment`