# muita-conta_devops

# 1. Criar um namespace dedicado para o Argo CD
kubectl create namespace argocd

# 2. Aplicar o manifesto de instalação oficial do Argo CD
kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml

# 3. Instalar o nginx
kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/main/deploy/static/provider/cloud/deploy.yaml

depois cria o arquivo argocd-ingress.yaml, e aponta o dominio para o ipPublico

