#### 1. If you do not use the nfs storage part, you will have to create the "/data/{mysql,wordpress}" folder on ```all the worker-nodes``` of your cluster
_here is the command :_
```sh
mkdir -p /data/{mysql,wordpress}
```

#### 2. Create namespace
First start by creating the namespace. The file is located in => "MiniProjetKubernetes/namespace.yaml"
```sh
kubectl apply -f namespace.yaml
```

#### 3. Create secret
Second you have to create the secret. The file is located in => "MiniProjetKubernetes/secret.yaml"
```sh
kubectl apply -f secret.yaml
```

#### For the ```ingress``` I used "ingressClassName: nginx"
