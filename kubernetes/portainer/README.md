<div align="center">
    <h1>Portainer</h1>
</div>

## Deployment

1. Add the Helm Repository

   ```bash
   helm repo add portainer https://portainer.github.io/k8s/
   ```

2. Create a namespace for Portainer

   ```bash
    kubectl create namespace portainer
   ```

3. Install Portainer

   ```bash
   helm upgrade --install --create-namespace -n portainer portainer portainer/portainer \
        --set enterpriseEdition.enabled=true \
        --set tls.force=true
   ```

   > **Note**: If you need to access Portainer via HTTP, remove the `--set tls.force=true` option.
