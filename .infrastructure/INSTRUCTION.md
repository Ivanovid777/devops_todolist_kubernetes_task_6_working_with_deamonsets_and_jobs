* how to deploy:
```bash
    kubectl create ns mateapp
    kubectl apply -f .infrastructure/daemonset.yml 
    kubectl apply -f .infrastructure/cronjob.yml 
```
* how to check:
```bash
    kubectl logs cronfortodoapp<name-pod-cron> -n mateapp
    kubectl logs daemonset<name-pod-daemonset> -n mateapp
