# Description

Version: 1.0.28

This template deploys Turbine server provided by Kubeflix project. See project documentation [here](https://github.com/fabric8io/kubeflix/blob/v1.0.28/readme.md#turbine-server).

# Requirements

This application uses OpenShift ConfigMap. In order to access it view permission is required. Enable it as follows:

    oc policy add-role-to-user view system:serviceaccount:$(oc project -q):turbine-server
