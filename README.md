# KRAKEN Deploy Controlm

Dashboard estático para GitHub Pages que simula:
- Pipeline GitHub Actions → Docker → Amazon ECR → DEV/CERT/PROD.
- Arquitectura AWS de referencia: Route 53, CloudFront, WAF, ALB, ECS/EKS, Redis opcional, RDS/Aurora Multi-AZ.
- Request trace web→DB→respuesta.
- Failure injection y rollback simulados.

## Publicar en GitHub Pages
1. Sube `index.html` a la raíz del repositorio.
2. En GitHub: Settings → Pages.
3. Selecciona Deploy from a branch → `main` → `/root`.
4. Guarda y espera el deploy.

**Demo visual:** no autentica en GitHub ni despliega recursos reales en AWS. Para eso habría que agregar workflow de GitHub Actions, AWS OIDC y configuración real de infraestructura.
