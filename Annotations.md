#### Manipulando o cluster

 `minikube status`

 `minikube start`

 `minikube delete`

`minikube service frontend-svc --url`

` minikube service frontend-svc `

`minikube service frontend-svc`

`minikube dashboard`

## kubectl 

#### Listando informações

 `kubectl get pods`

 `kubectl get pods -o wide`

 `kubectl describe pod`

 `kubectl describe pod nginx-server`

 `kubectl describe replicaset name-rs`

 `kubectl describe deployment name-dp`

 `kubectl get replicaset`

 `kubectl get replicationcontroller`

 `kubectl get deployment`

 `kubectl get all`

 `kubectl rollout status deployment/frontend-dp`

 `kubectl rollout history deployment/frontend-dp`  

`kubectl get namespace` | `kubectl get ns`

`kubecl get pods -n thenamespace`

#### Executando ações

`kubectl set image deployment frontend-dp frontend-container=nginx:1.18 --record`

`kubectl run nginx-server --image=nginx`

 `kubectl delete pod nginx-server`

 `kubectl delete replicaset nome-rs`

 `kubectl delete replicationcontroller nome-rc`

 `kubectl create -f pod.yaml`

 `kubectl create -f pod.yaml --save-config`

 `kubectl create -f pod.yaml --save-config --record`

`kubectl create -f pod.yaml --save-config --namespace=frontend`

`kubectl create -f namespaces/backend.yaml --save-config`

 `kubectl apply -f pod.yaml`

 `kubectl scale replicaset frontend-rs --replicas=4`

`kubectl scale deployment frontend-dp --replicas=10`

 `kubectl rollback undo deployment frontend-dp`

`kubectl rollback undo deployment frontend-dp --to-revision=2`

`kubectl describe service kubernetes`

`kubectl config set-context --current --namespace=frontend`







#### Alguns termos para lembrar

> ScaleUp/ScaleDown
> Rolling Release/Rolling Update
> Rollout
> Estrategia Recreate (ñ default) - Derruba todos pods de uma vez
> Rolling Update (default) - Atualiza um a um

