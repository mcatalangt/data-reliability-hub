# Bienvenido al Data Reliability Hub

**Data Reliability Hub** es una biblioteca integral de módulos de Terraform y Ansible, agnósticos a la nube/on-prem listos para producción.

Diseñado para ingenieros que buscan excelencia, este hub permite desplegar desde entornos de pruebas (Sandbox) hasta arquitecturas de **Alta Disponibilidad** (HA) en cuestión de minutos. 

Todo el código sigue rigurosamente las mejores prácticas de **SRE**, **DevSecOps** e **Ingeniería de Datos**, garantizando infraestructuras seguras y resilientes desde el primer despliegue.

Muchas de las buenas practicas y herramientas son parte del Cloud Native Landscape


##Cloud Native Landscape

es el "mapa" oficial mantenido por la **CNCF (Cloud Native Computing Foundation)** que organiza el inmenso ecosistema de herramientas necesarias para construir, desplegar y gestionar aplicaciones modernas en la nube.

En resumen, es la guía definitiva para pasar de servidores tradicionales a arquitecturas de microservicios, contenedores y automatización.

Para **Data Reliability Hub**, el landscape se divide en capas clave:

###1. Provisioning (infraestructura Core)

**Qué hace:** Crea y endurece la base sobre la que corren las apps.

**Herramientas clave:** Terraform (Automatización), Ansible, Keycloak (Seguridad/Identidad).

1. Runtime (El Motor)
Entorno donde se ejecutan los contenedores.

Qué hace: Gestiona el almacenamiento, la red y la ejecución de contenedores.

Herramientas clave: Kubernetes (Orquestación), Containerd, CRI-O.

3. Orchestration & Management (El Cerebro)
Cómo se conectan y descubren los servicios.

Qué hace: Service Mesh, descubrimiento de servicios y coordinación.

Herramientas clave: Istio, CoreDNS, etcd, Envoy.

4. App Definition & Development (El Flujo)
Herramientas para desarrolladores y pipelines.

Qué hace: CI/CD, bases de datos y gestión de imágenes.

Herramientas clave: ArgoCD, Helm, GitLab CI, Harbor.

5. Observability & Analysis (Los Ojos del SRE)

Qué hace: Monitoreo, Logging y Tracing para saber qué pasa en tiempo real.

Herramientas clave: Prometheus, Grafana, ELK Stack (Elasticsearch, Logstash, Kibana), Jaeger.

![Cloud Native Landscape](assets/landscape.png){ align=center width="100%" }