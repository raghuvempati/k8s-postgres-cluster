# PostgreSQL cluster on Kubernetes

The goal is to host an open source database on Kubernetes cluster with persistence.

This can be achieved using two distinct concepts of Kubernetes: Deployment and Statefulset.

This has been implemented using Minikube.

## Using Deployment

Use the following files preferably in this order:

* configmap.yaml
* storage.yaml
* service.yaml
* deployment.yaml

## Using Statefulset

Use the following files preferably in this order:

* configmap.yaml
* service.yaml
* statefulset.yaml

Note: For StatefulSet, in Minikube, you can dynamically provision the persistent volume and hence don't need to create the storage explicitly.

# References

* Kubernetes Documentation: https://kubernetes.io/docs/home/
* PostgreSQL cluster using StatefulSets: https://kubernetes.io/blog/2017/02/postgresql-clusters-kubernetes-statefulsets
* Using Kubernetes to Deploy PostgreSQL: https://severalnines.com/blog/using-kubernetes-deploy-postgresql
