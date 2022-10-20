
## usage

kpt pkg get github.com/yndd/yndd-packages.git
kpt fn render

## add namespace

mkdir namespace
kpt pkg init namespace
-> add namespace to Kptfile
kptgen apply namespace ./namespace 
rm namespace/package-context.yaml

## add crds of yndd core packages

kpt pkg get https://github.com/henderiw-nephio/admin/blueprint/admin@v0.0.4 admin kpt pkg get

kpt pkg get https://github.com/yndd/target/blueprint/target/crd@v0.0.110 target-crd kpt pkg get
kpt pkg get https://github.com/yndd/topology/blueprint/topology/crd@v0.0.20 topology-crd kpt pkg get
kpt pkg get https://github.com/yndd/discovery/blueprint/discovery/crd@v0.0.4 discovery-crd kpt pkg get

kpt pkg update admin@v0.0.7