# SRE - Infrastructure as Code (IaC)

Esta sección centraliza plantillas de **Terraform** diseñadas para desplegar infraestructura segura y compatible con HIPAA en Google Cloud y AWS.

## Arquitectura
El código está modularizado para permitir la reutilización en diferentes entornos (Dev, Staging, Prod) asi como Cloud y On Prem.

!!! info "Stack Tecnológico"
    * **Cloud:** Google Cloud Platform (GCP)
    * **Herramienta:** Terraform v1.5+, Ansible, GitHub, GitHub Actions, Github Package
    * **Seguridad:** IAM Least Privilege, VPC Service Controls

## Acceso al Código

El código fuente completo se encuentra en el submódulo `data-reliability-hub` nuestro repositorio central.

[Ver Código Fuente en GitHub :octicons-link-external-16:](https://github.com/mcatalangt/data-reliability-hub){ .md-button .md-button--primary }

---

### Módulos Incluidos

| Módulo | Descripción | Estado | Repositorio |
| :--- | :--- | :---: | :--- |
| `01-iac-postgresql` | Despliegue de BD PostgreSQL en GCE. | ✅ Stable | [GitHub :octicons-link-external-16:](https://github.com/mcatalangt/data-reliability-hub/tree/main/01-iac-postgresql) |
| `02-iac-prefect` | Despliegue de Workflow tool Prefect en GCE. | 🚧 Beta | [GitHub :octicons-link-external-16:](https://github.com/mcatalangt/data-reliability-hub/tree/main/02-iac-prefect) |
| `03-iac-event-driven` | Despliegue de event driven (PubSub, Kafka, RabbitMQ). | 🚧 Beta | [GitHub :octicons-link-external-16:](https://github.com/mcatalangt/data-reliability-hub/tree/main/03-iac-event-driven) |
| `04-iac-kubernetes` | Despliegue de Kubernetes en GKE. | ✅ Stable | [GitHub :octicons-link-external-16:](https://github.com/mcatalangt/data-reliability-hub/tree/main/04-iac-kubernetes) |
| `05-iac-observability` | Despliegue de Grafana Stack en GKE. | ✅ Beta | [GitHub :octicons-link-external-16:](https://github.com/mcatalangt/data-reliability-hub/tree/main/05-iac-observability) |