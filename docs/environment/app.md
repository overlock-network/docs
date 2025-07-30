---
id: cfg-file
title: Configuration file 
sidebar_position: 0
---

# Environment configuration file 

Overlock enables you to define and manage your local development environment using a declarative YAML configuration file (by default, `overlock.yaml`). This approach makes it easy to version-control, reload, and share reproducible setups. The configuration covers networking, Kubernetes runtime, storage mounts, and lists of Providers, Configurations, and Functions that are automatically applied when the environment is created. This is ideal for restoring environments after a restart or collaborating with others.

```yaml
# HTTP port mapping for the environment (default: 80)
httpport: 80

# HTTPS port mapping for the environment (default: 443)
httpsport: 443

# Kubernetes context where the environment will be created
context: "my-k8s-context"

# Kubernetes engine for the runtime environment (default: "kind")
# Supported values: "kind", "k3s", "k3d"
engine: "kind"

# Path to the engine configuration file (supported for kind clusters)
engineconfig: "/path/to/kind-config.yaml"

# Host directory to mount at /storage (optional)
mountpath: "/host/storage/path"

# Providers to apply to the environment
providers:
    - "xpkg.upbound.io/upbound/provider-family-aws:v1"
    - "xpkg.upbound.io/upbound/provider-family-gcp:v1"

# Configurations to apply to the environment
configurations:
    - "xpkg.upbound.io/upbound/platform-ref-aws:v1.4.0"
    - "xpkg.upbound.io/upbound/platform-ref-azure:v0.14.0"

# Functions to apply to the environment
functions:
    - "xpkg.upbound.io/upbound/function-go-templating:v0.10.0"
    - "xxpkg.upbound.io/crossplane-contrib/function-kcl:v0.11.4"
```