# kubernetes statefulset mysql single
statefulset mysql on gcp (higher availability with regional zones: asia-southeast1-a, asia-southeast1-b persistent disks)


## run config secret pass for mysql ##
kubectl create secret generic mysql-dev-pass --from-literal=password=joe123

## deploy mysql server ##
kubectl apply -f mysql.yaml


Note: make sure your cluster GKE run Regional not Single Zone (singapore)