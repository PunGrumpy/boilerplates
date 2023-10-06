<div align="center">
    <h1>Cert Manager</h1>
</div>

## Deployment

1. Add the Helm Repository

   ```bash
   helm repo add traefik https://traefik.github.io/charts
   ```

2. Update the Helm Repository

   ```bash
   helm repo update
   ```

3. Install the Helm Chart

   ```bash
   helm install traefik traefik/traefik
   ```
