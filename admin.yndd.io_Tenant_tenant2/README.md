# admin.yndd.io_Tenant_tenant2

## Description
admin.yndd.io_Tenant_tenant2

## Usage

### Fetch the package
`kpt pkg get REPO_URI[.git]/PKG_PATH[@VERSION] admin.yndd.io_Tenant_tenant2`
Details: https://kpt.dev/reference/cli/pkg/get/

### View package content
`kpt pkg tree admin.yndd.io_Tenant_tenant2`
Details: https://kpt.dev/reference/cli/pkg/tree/

### Apply the package
```
kpt live init admin.yndd.io_Tenant_tenant2
kpt live apply admin.yndd.io_Tenant_tenant2 --reconcile-timeout=2m --output=table
```
Details: https://kpt.dev/reference/cli/live/
