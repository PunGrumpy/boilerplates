<div align="center">
    <h1>Cert Manager</h1>
</div>

## Installation

### Helm

```bash
# Add Repository
helm repo add jetstack https://charts.jetstack.io

# Update Repository
helm repo update

# Install
helm install cert-manager jetstack/cert-manager \
    --namespace cert-manager \
    --create-namespace \
    --version v1.13.1 \
    --set installCRDs=true
```

## Templates

[templates](templates/)
