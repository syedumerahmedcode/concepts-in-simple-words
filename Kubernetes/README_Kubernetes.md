# Kubernetes

How to set up deployment of an artifact in Kubernetes.

- A new folder for the artifact in the deployment environments(dev, qa, staging, prod).
- Ingress in case there needs to a separate host for each environment. (Prerequisite: There should be DNS entry for each environment).
- a secret docker registry(if applicable)
- Prometheus(if it is used in the organization)
- Changes in Helm(if Helm is used). Otherwise change the resources directly in flux as it saves the developer a Helm release.
- Namespace(per environment)
- Persistance Volume Claim(In case a file is saved on disk. Otherwise, not).
- Secerts
- ConfigMaps
- Services
- Deployments
 