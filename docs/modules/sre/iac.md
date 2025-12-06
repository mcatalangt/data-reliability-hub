# SRE IAC

# Infrastructure as Code (IaC)

Este módulo centraliza las plantillas de **Terraform** diseñadas para desplegar infraestructura segura y compatible con HIPAA en Google Cloud y AWS.

## 🏗️ Arquitectura
El código está modularizado para permitir la reutilización en diferentes entornos (Dev, Staging, Prod).

!!! info "Stack Tecnológico"
    * **Cloud:** Google Cloud Platform (GCP)
    * **Herramienta:** Terraform v1.5+
    * **Seguridad:** IAM Least Privilege, VPC Service Controls

## 📂 Acceso al Código

El código fuente completo se encuentra en el submódulo `01-infrastructure-as-code` de nuestro repositorio central.

[Ver Código Fuente en GitHub :octicons-link-external-16:](https://github.com/mcatalangt/data-reliability-hub/tree/main/01-infrastructure-as-code){ .md-button .md-button--primary }

---

### Módulos Incluidos

| Módulo | Descripción | Estado |
| :--- | :--- | :---: |
| `gcp-secure-baseline` | Configuración base de red y seguridad IAM. | ✅ Stable |
| `aws-network-hub` | Arquitectura Hub-and-Spoke para VPCs. | 🚧 Beta |