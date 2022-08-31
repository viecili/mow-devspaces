# Managed OpenShift Workshop - DevSpaces 


## Bootstrap Dev Spaces
### Pre-requisites
* `oc` cli
* `dsc` cli from https://developers.redhat.com/products/openshift-dev-spaces/download

Note: last tested with DevSpaces 3.1

### Deploy DevSpaces Server

Log in to OpenShift

```zsh
export OC_API=
export OC_USER=kubeadmin
oc login -u $OC_USER --server=$OC_API
```

Deploy to OpenShift

```
dsc server:deploy --platform openshift --telemetry=off --no-auto-update
# if it fails, try again (it usually works) - takes ~5min to finish
```

 The command below shows the url that should be given to students to start up their workspace:

```zsh
echo "https://`oc get route devspaces -o jsonpath='{.spec.host}'`/f?url=https://github.com/viecili/mow-devspaces"
```

Optionally, open https://hub.int.us-east.dc.prod.paas.redhat.com/urls/redht and create a custom red.ht URL. (VPN required)

