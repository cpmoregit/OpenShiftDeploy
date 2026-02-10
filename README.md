# OpenShiftDeploy

## Check Resourcetype that a ClusterRole can apply in OpenShift
oc api-resources --verbs=list --namespaced=false

## Create Role
1. Update Role Using createrole.yaml
2. Apply role
   oc apply -f yaml/createrole.yaml
3. Check Role
   oc get role xxxrole -n <namespace

 ClusterRole applies to all namespaces in the cluster, allowing you to manage permissions for resources across the entire cluster.

 > Note: When users are granted get permissions for the pods/* endpoints, the users are permitted to use all Pod subresources, including the Web Terminal or port-forwarding. This also applies to the following Pod subresources:
pods/attach
pods/exec
pods/portforward
pods/proxy
pods/log
pods/status
