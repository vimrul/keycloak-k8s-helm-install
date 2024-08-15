# keycloak-k8s-helm-install
Keycloak installation on Kubernetes using Helm but not relying on Helm charts

# create secret regcred

kubectl create secret docker-registry regcred \
    --docker-server=https://index.docker.io/v1/ \
    --docker-username=<your-docker-username> \
    --docker-password=<your-docker-password> \
    --docker-email=<your-email> \
    -n keycloak

