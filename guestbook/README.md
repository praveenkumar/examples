# Example: Guestbook application on Kubernetes/OpenShift

This directory contains the source code and Kubernetes/OpenShift manifests for PHP
Guestbook application.

You can try it on CRC(https://github.com/crc-org/crc/releases) using microshift preset.
```
$ crc config set preset microshift
$ crc setup
$ crc start

$ oc create namespace demo
$ oc config set-context --current --namespace=demo
$ oc apply -f  https://raw.githubusercontent.com/praveenkumar/examples/master/guestbook/all-in-one/guestbook-all-in-one.yaml
$ oc expose svc frontent
$ oc get routes
```

