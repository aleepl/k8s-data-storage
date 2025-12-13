helm-add-operator-repo:
	helm repo add minio-operator https://operator.min.io

k8s-create-namespaces:
	kubectl apply -f ./kubernetes/namespaces.yaml

helm-install-operator:
	helm install operator minio-operator/minio-operator --namespace minio-operator -f ./helm/chart/operator-values.yaml

helm-install-tenant:
	helm install tenant minio-operator/tenant --namespace minio-tenant -f ./helm/chart/tenant-values.yaml