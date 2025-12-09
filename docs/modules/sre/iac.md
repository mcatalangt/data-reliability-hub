# SRE - Infrastructure as Code (IaC)

Esta sección centraliza plantillas de :simple-terraform: [Terraform](https://www.terraform.io/) diseñadas para desplegar infraestructura segura y compatible con HIPAA en :simple-googlecloud: [Google Cloud](https://cloud.google.com/), AWS y On-Prem.

## Arquitectura
El código está modularizado para permitir la reutilización en diferentes entornos (Dev, Staging, Prod) asi como Cloud y On-Prem.

!!! info "Stack Tecnológico"
    * **Cloud:** Google Cloud Platform (GCP)
    * **Herramienta:** Terraform v1.5+, Ansible, GitHub, GitHub Actions, Github Package
    * **Seguridad:** IAM Least Privilege, VPC Service Controls

## Acceso al Código

El código fuente completo se encuentra en el submódulo `data-reliability-hub` nuestro repositorio central.

[Código Fuente en GitHub :octicons-link-external-16:](https://github.com/mcatalangt/data-reliability-hub){ .md-button  }

---

### Módulos Incluidos

| Módulo | Descripción | Caso de uso |Estado | Repositorio |
| :----: | :--- | :---: | :--- | :--- |
| `01-iac-postgresql` | Creación de BD PostgreSQL. | Base de datos para pruebas. | ✅ Stable | [GitHub :octicons-link-external-16:](https://github.com/mcatalangt/data-reliability-hub/tree/main/01-iac-postgresql) |
| `02-iac-prefect` | Creación de Workflow Prefect. | Orquestador y Automatizador de flujos de trabajo| 🚧 Beta | [GitHub :octicons-link-external-16:](https://github.com/mcatalangt/data-reliability-hub/tree/main/02-iac-prefect) |
| `03-iac-event-driven` | Creación de event driven (PubSub, Kafka, RabbitMQ). |Gestion de mensajes y desacoplamiento de sistemas| 🚧 Beta | [GitHub :octicons-link-external-16:](https://github.com/mcatalangt/data-reliability-hub/tree/main/03-iac-event-driven) |
| `04-iac-kubernetes` | Creación de Kubernetes en GKE. | Orquestador de Contenedores en 5 minutos| ✅ Stable | [GitHub :octicons-link-external-16:](https://github.com/mcatalangt/data-reliability-hub/tree/main/04-iac-kubernetes) |
| `05-iac-observability` | Creación de Grafana Stack en GKE. | Observabilidad de sistemas transacionales E2E (Logs, Trazas, Metricas y Perfiles)| 🚧 Beta | [GitHub :octicons-link-external-16:](https://github.com/mcatalangt/data-reliability-hub/tree/main/05-iac-observability) |