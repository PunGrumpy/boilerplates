<div align="center">
    <h1>Cert Manager</h1>
</div>

## Deployment

1. Add the Helm Repository

   ```bash
   helm repo add jetstack https://charts.jetstack.io
   ```

2. Update the Helm Repository

   ```bash
   helm repo update
   ```

3. Install the Helm Chart

   ```bash
   helm install cert-manager jetstack/cert-manager \
     --namespace cert-manager \
     --version v1.13.1
     --create-namespace \
     --set installCRDs=true
   ```

## Configuration

Add `Issuer` or `ClusterIssuer`, `Credential` and `Certificate` resources to the `cert-manager` namespace.

For more information, see the [cert-manager documentation](https://cert-manager.io/docs/).
