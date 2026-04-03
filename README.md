# Affinity-Taint-Jobs-Tolerance

## Commands:

kubectl get no
kubectl create -f node-affinity.yml
kubectl label node nodeid app=swiggy
kubectl get po -o wide


kubectl create -f pod-affinity.yml
kubectl get po -o wide

kubectl create -f db-pod.yml
kubectl get po -o wide


kubectl create -f pod-anti-affinity.yml
kubectl get po -o wide


kubectl taint node nodeid env=prod:NoSchedule
kubectl describe node nodeid | grep -i "taint"

kubectl create -f job.yml
kubectl get jobs
kubectl get po
kubectl get po -o wide


kubectl create -f cronjob.yml
kubectk get cj
kubectl get po
kubectl get po -o wide

