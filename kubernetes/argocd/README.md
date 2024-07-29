<div align="center">
    <h1>Argo CD</h1>
</div>

### Deployment

1. Add the Helm Repository

   ```bash
   helm repo add argo https://argoproj.github.io/argo-helm
   ```

2. Update the Helm Repository

   ```bash
    helm repo update
   ```

3. Install the Helm Chart

   ```bash
   helm install argo argo/argo-cd
   ```

4. Get the Argo CD password

   ```bash
    kubectl -n argocd get secret argocd-initial-admin-secret -o jsonpath="{.data.password}" | base64 -d
   ```

5. Port forward the Argo CD UI

   ```bash
   kubectl port-forward svc/argo-argo-cd 8080:80 -n argocd
   ```

6. Access the Argo CD UI

   ```bash
   open http://localhost:8080
   ```

7. Login with the username `admin` and the password from step 4

8. Change the password

   ```bash
   argocd account update-password
   ```
