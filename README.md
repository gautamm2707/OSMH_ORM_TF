# OSMH Resource Manager Terraform

This repository contains the standalone Oracle Cloud Infrastructure Resource Manager stack for scheduled OS Management Hub onboarding.

## Deploy

[Onboard in OSMH](https://cloud.oracle.com/resourcemanager/stacks/create?zipUrl=https%3A%2F%2Fgithub.com%2Fgautamm2707%2FOSMH_ORM_TF%2Fraw%2Frefs%2Fheads%2Fmain%2Fresource-manager%2Fosmh-resource-manager.zip)

The button opens OCI Resource Manager with the published ZIP. Review the variables, run **Plan**, and then run **Apply**.

## Package contents

The package is generated from the explicit allowlist in `package_resource_manager.py`. Terraform files, the OCI Console schema, DevOps build definition, Function sources, runtime helpers, and deployment documentation are stored at the repository root and under `function/`.

Generate the package locally with:

```bash
python3 package_resource_manager.py --output resource-manager/osmh-resource-manager.zip
```

See `BLOG.md` for the deployment workflow and `RESOURCE_MANAGER.md` for implementation and recovery details.
