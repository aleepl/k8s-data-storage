helm-add-cnpg:
	helm repo add cnpg https://cloudnative-pg.github.io/charts

k8s-install-cnpg:
	kubectl apply -f namespace.yaml
	helm upgrade --install cnpg-operator cnpg/cloudnative-pg --namespace cnpg-system --version 0.27.0