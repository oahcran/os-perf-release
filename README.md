# os-perf-release
Cloud Foundry BOSH Release for OS Tuning

## Implementation

```
bosh init release os-perf-release
cd os-perf-release
bosh generate job kernel_network
```

## Release

```
git clone
cd os-perf-release
bosh create release --force
bosh create release --force --final
bosh upload release
```

Deploy as a BOSH Add-on

## Validation

```
cat /proc/sys/net/core/wmem_max
```
