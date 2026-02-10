# OpenShiftDeploy

## Create Role
1. Update Role Using createrole.yaml
2. Apply role
   oc apply -f yaml/createrole.yaml
3. Check Role
   oc get role xxxrole -n <namespace

