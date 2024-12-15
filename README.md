# argocd_training_2024_code
kubectl.exe  create sa staging-cluster-sa

kubectl.exe  create clusterrolebinding  staging-cluster-sa-rolebn --clusterrole=cluster-admin  --serviceaccount=default:staging-cluster-sa


kubectl.exe  create token staging-cluster-sa





kubectl.exe  config   use-context  argocluster


kubectl.exe  config   use-context  prodcluster


kubectl.exe  create sa prod-cluster-sa

kubectl.exe  create clusterrolebinding  prod-cluster-sa-rolebn --clusterrole=cluster-admin  --serviceaccount=default:prod-cluster-sa



kubectl.exe  create token prod-cluster-sa



