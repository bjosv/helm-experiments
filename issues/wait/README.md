# Upgrade/install with --wait is not always working

## Fix exists in:
https://github.com/helm/helm/pull/10920

## Build
```
git fetch origin pull/10920/head:PR10920
git co PR10920
make build

./bin/helm upgrade my-release --install --wait --debug <CHART_PATH>
```
Charts:
- helmchart-replicaset
- helmchart-replicationcontroller
