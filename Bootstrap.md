# Managed OpenShift Workshop - DevSpaces 


## Bootstrap Dev Spaces
### Pre-requisites
* `oc` cli
* `dsc` cli from https://developers.redhat.com/products/openshift-dev-spaces/download

Note: last tested with DevSpaces 3.1

### Deploy DevSpaces Server
```zsh
# export OC_API=
# export OC_USER=kubeadmin
# oc login -u $OC_USER --server=$OC_API
dsc server:deploy --platform openshift --telemetry=off --no-auto-update
# if it fails, try again (it usually works) - takes ~ 5min to finish
# the command below shows the url that should be given to students to start up they workspace
echo "https://`oc get route devspaces -o jsonpath='{.spec.host}'`/f?url=https://github.com/viecili/mow-devspaces"
```


