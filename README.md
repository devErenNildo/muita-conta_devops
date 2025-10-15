# muita-conta_devops

# 1. Criar um namespace dedicado para o Argo CD
kubectl create namespace argocd

# 2. Aplicar o manifesto de instalação oficial do Argo CD
kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml

# 3. Editar o server para loadbalance para expor um ip para ser acessado
kubectl edit service/argocd-server -n argocd
