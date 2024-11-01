# Bootstrap & Configure ArgoCD

## Enable the OpenShift GitOps operator on the cluster

`oc apply -k gitops/bootstrap`

## Deploy the instance of OpenShift GitOps (ArgoCD)
- Create the `local-cluster` Argo project
- Configure rbac role

`oc apply -k gitops/setup`

## Enable additional Operators on the cluster using ArgoCD

`oc apply -f gitops/operator-appset.yaml`
